# PhpLaravel_Install
php, laravel framwork install

Step 1: Add PHP 7.3 Remi repository
---------------------------------------
sudo yum -y install http://rpms.remirepo.net/enterprise/remi-release-7.rpm 

sudo yum -y install epel-release yum-utils


Step 2: Disable repo for PHP 5.4
------------------------------------

sudo yum-config-manager --disable remi-php54

sudo yum-config-manager --enable remi-php73

Step 3: How to Install PHP 7.3 on CentOS 7 / Fedora
-------------------------------------------------------

sudo yum -y install php php-cli php-fpm php-mysqlnd php-zip php-devel php-gd php-mcrypt php-mbstring php-curl php-xml php-pear php-bcmath php-json

sudo yum install php-mysql

php -v



Composer Installation:
-----------------------------
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"

php -r "if (hash_file('sha384', 'composer-setup.php') === '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"

php composer-setup.php

php -r "unlink('composer-setup.php');"

sudo mv composer.phar /usr/local/bin/composer

composer


Laravel Installation:
----------------------------

composer global require laravel/installer
