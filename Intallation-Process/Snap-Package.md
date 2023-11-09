**Snap Install**
```
$ sudo apt install snapd
```

```
$ sudo snap version
```

```
$ sudo snap install nextcloud
```

```
$ sudo snap list
```

First, configure Uncomplicated Firewall (UFW) to allow HTTP network traffic on the server port 80.

 $ sudo ufw allow 80/tcp
Allow HTTPS on port 443.

 $ sudo ufw allow 443/tcp
Restart the Firewall.

 $ sudo ufw reload
To activate the NextCloud database and configuration file values, visit your Server IP using a web browser.

 http://192.0.2.1
Enter a username and strong password to create the first administrator account, and click Install.

NextCloud Snap installation page

Close the web browser and switch to your server console.

Using a text editor of your choice, edit the main NextCloud configuration file.

 $ sudo nano /var/snap/nextcloud/current/nextcloud/config/config.php
Find the "trusted_domains' =>` section, and replace the Server IP with your domain name as below.

 'trusted_domains' =>
    array (
       0 => 'nextcloud.example.com',
     ),
Save and close the file.