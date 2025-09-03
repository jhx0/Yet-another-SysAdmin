## Setting up phpSysInfo

### Howto
1. Install everything needed (Webserver, PHP, PHP extension) via APT
```
$ sudo apt install -y apache2 libapache2-mod-php php-xml
```
2. Downloading the newest tar archive
```
$ cd /var/www/html
$ wget https://github.com/phpsysinfo/phpsysinfo/archive/refs/tags/v3.4.4.tar.gz
```
3. Setting up phpSysInfo   
```
$ sudo rm index.html
$ sudo tar xf v3.4.4.tar.gz
$ cd phpsysinfo-3.4.4/
$ sudo mv * ../
$ sudo mv .* ../
$ sudo rmdir phpsysinfo-3.4.4/
$ sudo mv phpsysinfo.ini.new phpsysinfo.ini
$ sudo chown www-data:www-data . -hR
```
4. Viewing the site
```
$ firefox $IP_ADDR
```
Note: You might want to make a entry in your /etc/hosts file or use DNS server of choice to add a A record. (If you for example host phpSysInfo on one of your servers)
This is of course up to the user and the use case.