### ssh
- ssh-keygen -t ecdsa
- ls ~/.ssh
- cat .ssh/id_ecdsa.pub
- copy ssh into your hosting platform, there is gonna ip address we could use
```
  example ip address from hosting provider
  $ssh root@167.71.255.125

```
- ifconfig, check the inet
```
ssh: /etc/ssh/sshd_config
nginx: /etc/nginx/{nginx.conf,conf.d}
mysql: /etc/mysql/mysql.cnf
php: /etc/php8/fpm/php.ini

```

  
### linux user
- ssh root@167.71.255.125
- adduser websiteuser
- su - websiteuser
- whoami


### nginx
- less /usr/share/nginx/html/index.html, is welcome page nginx
- mkdir -p /usr/share/nginx/cache/fcgi, for folder cache nginx
- nginx -t
- systemctl reload nginx

### mysql
- ssh root@167.71.255.125
- mysql_install_db, this is command for install mysql
- usr/bin/mysql_secure_installation
- systemctl restart mysql

### php
- apt-get install php
- mkdir /var/run/php-fpm
- mkdir -p /etc/php8/fpm/pool.d

### aws
- ssh -i something-example.pem ubuntu@34.209.206.172