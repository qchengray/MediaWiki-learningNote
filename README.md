# Install __MediaWiki__ on Ubuntu

## Depends <br>
* Apache
* PHP
* MySQL

#### Install depends 
```bash
## Terminal lines <br>
sudo apt-get install apache2 mysql-server php5 php5-mysql libapache2-mod-php5 <br>
## Ubuntu Xenial and Debian Stretch include PHP 7.0, and renamed many packages from "php5" to plain "php". In addition, some PHP modules are now in separate packages (xml, mbstring)
sudo apt-get install apache2 mysql-server php php-mysql libapache2-mod-php php-xml php-mbstring <br>
```

## Download MediaWiki and extract it
```bash
cd /home/malab4/Downloads
wget https://releases.wikimedia.org/mediawiki/1.28/mediawiki-1.28.0.tar.gz
## extract 
tar -xvzf /pathtofile/mediawiki-*.tar.gz
sudo mkdir /var/lib/mediawiki
sudo mv mediawiki-*/* /var/lib/mediawiki
```
