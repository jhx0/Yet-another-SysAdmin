## Using http on OpenBSD

### Howto
1. Edit the config file:
```
$ vi httpd.conf
```
2. Copy it over to /etc
3. Enable/Start httpd:   
```
$ rcctl enable httpd && rcctl start httpd
```

### Example
A more in depth example can be found here:
```
/etc/examples
```
(On any OpenBSD system)