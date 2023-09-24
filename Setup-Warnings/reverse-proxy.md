## Behind a reverse proxy and the overwrite config variables are not set correctly

1. add the following code to `config.php`

```php
'trusted_domains' => 
  array (
    0 => 'yourdomain.com',
  ),
  'trusted_proxies' => 
  array (
    0 => 'yourdomain.com',
  ),
  'overwrite.cli.url' => 'https://yourdomain.com',
  'overwriteprotocol' => 'https',
```
