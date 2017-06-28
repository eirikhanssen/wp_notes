# wp_notes
## Import/Export pages and posts
Use Wordpress Importer and Wordpress Exporter plugin.

## Switch php-versions:

### Use Ondrej PPA:
sudo add-apt-repository ppa:ondrej/php
sudo apt-get update
sudo apt-get install php7.0 php5.6 php5.6-mysql php-gettext php5.6-mbstring php-mbstring php7.0-mbstring php-xdebug libapache2-mod-php5.6 libapache2-mod-php7.0

### Switch from php5.6 to php7.0

#### Apache
sudo a2dismod php5.6 ; sudo a2enmod php7.0 ; sudo service apache2 restart

#### CLI
sudo update-alternatives --set php /usr/bin/php7.0


### Switch from php7.0 to php5.6

#### Apache
sudo a2dismod php7.0 ; sudo a2enmod php5.6 ; sudo service apache2 restart

#### CLI
sudo update-alternatives --set php /usr/bin/php5.6
