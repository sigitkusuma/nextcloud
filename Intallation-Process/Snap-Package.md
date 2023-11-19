# Nexcloud installation using Snap-Package

## Snap Installation Process
### Step 1: Install Snapd
   - Snapd is the service that manages Snap packages on your system. To install it, use the following command:
```
$ sudo apt install snapd
```

### Step 2: Enable Snapd Socket
- Some versions of Ubuntu may require you to enable the Snapd socket. You can do this with the following command:
```
$ sudo systemctl enable --now snapd.socket
```

### Step 3: Test Snap Installation
- To verify that Snapd is installed and working correctly, you can run a test command. 
- Try installing the hello-world snap package:
```
$ sudo snap install hello-world
```

- After the installation is complete, you can run the hello-world command to test the snap:
```
$ hello-world
```
- You should see a message indicating that the installation was successful.


## Nextcloud Installation Process
### Step 1: Install Nextcloud Snap Package
- Now, you can install Nextcloud using the Snap package:
```
$ sudo snap install nextcloud
```
- This command will download and install the Nextcloud snap package along with its dependencies.

### Step 2: Configure Nextcloud
- Once the installation is complete, you need to configure Nextcloud.
- By default, Nextcloud runs on server address.
- You can access it using web browser.
- Open your web browser and navigate to your server address. in this case my server address is http://192.168.1.7

- Follow the on-screen instructions to set up your Nextcloud instance. You will be asked to create an admin account and configure the database settings.
