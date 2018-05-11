## raspberry pi 3 b
![](https://www.raspberrypi.org/wp-content/uploads/2015/08/raspberry-pi-logo.png)

### แตกไฟล์ img ใส่ sd card
สำรวจหมายเลข disk
`diskutil list`

unmount disk
`diskutil unmountDisk /dev/disk3`

แตกไฟล์
`sudo dd bs=1m if=xxx.img of=/dev/rdisk3`

หมายเหตุ: ใช้ ctrl + T เพื่อเช็คความคืบหน้า

ใช้ `brew install xz``xz -d to-extract.xz` เพื่อแตกไฟล์ xz

credit: [แตกไฟล์ img ใส่ sd](https://www.raspberrypi.org/documentation/installation/installing-images/mac.md)


# Android on Rasp PI 3



## ติดตั้ง
https://www.youtube.com/watch?v=ddVY6OEpZlU

## ติดตั้ง Google Play
https://www.youtube.com/watch?v=iUc2oJuxk6E

### download  เอง
https://git.embedded.rwth-aachen.de/rtandroid/downloads/raspberry-pi/








### ref
[การเขียน Image File ของ RaspberryPi ลง SD-Card และขยายพื้นที่ให้เต็ม]
(https://www.unzeen.com/article/2151/)

[ต่อ External HDD กับ Raspberry Pi ให้กลายเป็น File Server ด้วย SAMBA]
(https://www.unzeen.com/article/2303/)

[ติดตั้ง Transmission BitTorrent Client สำหรับโหลดบิทบน Raspberry Pi]
(https://www.unzeen.com/article/2336/)

[Raspberry Pi - Media Center (ตอนที่ 1)]
(http://www.arduitronics.com/article/raspberry-pi-media-center-%E0%B8%95%E0%B8%AD%E0%B8%99%E0%B8%97%E0%B8%B5%E0%B9%88-1)
ทำ smart tv

[ubuntu mate]
(https://ubuntu-mate.org/raspberry-pi/)

[Turning the Raspberry Pi into a Wireless Access Point](http://www.thebitbangtheory.com/2012/12/turning-the-raspberry-pi-into-a-wireless-access-point/)

[USING YOUR NEW RASPBERRY PI 3 AS A WIFI ACCESS POINT WITH HOSTAPD](https://frillip.com/using-your-raspberry-pi-3-as-a-wifi-access-point-with-hostapd/)

## arduino
### esp8266
![](https://developer.mbed.org/media/uploads/4180_1/xesp8266.jpg.pagespeed.ic.N1E5_ap8jA.jpg)
[ESP8266 core for Arduino](https://github.com/esp8266/Arduino) ส่ง GET ได้

### ESP8266-12E (with new AT)
![](http://www.thaieasyelec.com/products/wireless-modules/wifi-modules/esp8266-12e-wifi-serial-transceiver-module-detail.html)

![](http://www.thaieasyelec.com/downloads/EFDV451/4B-ESP8266__AT%20Command%20Examples__EN_v0.4.pdf)


## angular
[รวบรวม ExpressJs Middleware ที่ควรใช้สำหรับมือใหม่สาย Full Stack Dev](https://www.algorithmtut.com/%E0%B8%A3%E0%B8%A7%E0%B8%9A%E0%B8%A3%E0%B8%A7%E0%B8%A1-expressjs-middleware-%E0%B8%97%E0%B8%B5%E0%B9%88%E0%B8%84%E0%B8%A7%E0%B8%A3%E0%B9%83%E0%B8%8A%E0%B9%89%E0%B8%AA%E0%B8%B3%E0%B8%AB%E0%B8%A3/)

## ionic
![](https://s3.amazonaws.com/media-p.slid.es/uploads/319342/images/1412723/ionic.png)

### ref
[push gcm](http://www.sitepoint.com/push-notifications-in-ionic-apps-with-google-cloud-messaging/)



## hold punching
http://stackoverflow.com/questions/27129268/udp-hole-punching-java-example

#### [github api](https://developer.github.com/v3/)
#### [JSON IP](http://www.telize.com/)


### Android
#### Retrofit 2 android
[Android Retrofit Images Tutorial](http://themakeinfo.com/2015/04/retrofit-android-tutorial/)

#### Picasso
[http://themakeinfo.com/2015/04/android-retrofit-images-tutorial/](http://themakeinfo.com/2015/04/android-retrofit-images-tutorial/)



# AngularJS
[angular-dashboard-framework](https://github.com/angular-dashboard-framework/)
## jQuery
[jq datatable](https://datatables.net)
[jq datatable button (extension)](https://datatables.net/extensions/buttons/)





# Mikrotik


## ติดตั้ง syslog-ng เอง
http://raspberry-pi-thai.blogspot.com/2014/09/syslog-ng-log-mikrotik-raspberry-pi.html

sudo service syslog-ng restart

tail -f /var/log/router.log

## อ่านผ่านๆ อีกที
http://www.sysnetcenter.com/board/index.php?topic=1582.0
http://www.wifi4you.com/Amp/%E0%B8%A7%E0%B8%B4%E0%B8%98%E0%B8%B5%E0%B8%81%E0%B8%B2%E0%B8%A3%E0%B9%80%E0%B8%81%E0%B9%87%E0%B8%9A-log-file-%E0%B8%88%E0%B8%B2%E0%B8%81-Mikrotik-%E0%B9%82%E0%B8%94%E0%B8%A2-NSA210.html


## Web Proxy (มีสอนโค้ด 55)
http://www.sysnetcenter.com/board/index.php?topic=2455.0







# SSL
[Github](https://github.com/certbot/certbot)

`./certbot-auto certonly --manual -d example.com -d www.example.com -d other.example.net`


### Note: https://certbot.eff.org/docs/using.html#manual  if encounter Timeout problem

## Set Key location
[](https://www.digitalocean.com/community/tutorials/how-to-create-a-ssl-certificate-on-apache-for-ubuntu-14-04)

`sudo a2enmod ssl`

`sudo service apache2 restart`

And edit
`sudo nano /etc/apache2/sites-available/default-ssl.conf`

Activate SSL Virtual Host
`sudo a2ensite default-ssl.conf`

Cron auto renew
[https://www.vultr.com/docs/setup-lets-encrypt-with-apache-on-ubuntu-16-04]


Redirect http to https
[https://www.digitalocean.com/community/questions/redirect-from-http-to-https]

`sudo a2enmod rewrite`

`
RewriteEngine On

RewriteCond %{HTTPS} off

RewriteRule (.*) https://%{HTTPHOST}%{REQUESTURI}
`

### Auto renew

`./certbot-auto renew`



คีย์จะอยู่ใน

`/etc/letsencrypt/live`


# Email (Postfix – Dovecot - Squirrelmail)
See this: [http://www.krizna.com/ubuntu/setup-mail-server-ubuntu-14-04/#postfix]
### Note in Step 15, don't forget to locate key and cur
and see more on:
[https://www.tecmint.com/setup-postfix-mail-server-in-ubuntu-debian/]





# Owncloud
(Official Installation)[https://doc.owncloud.org/server/latest/admin_manual/installation/source_installation.html]

Just download .zip,  unzip,  and run!!

See more:

https://devops.profitbricks.com/tutorials/install-and-configure-owncloud-on-ubuntu-1604/

https://www.digitalocean.com/community/tutorials/how-to-install-and-configure-owncloud-on-ubuntu-16-04


### Note: permission issue see this https://askubuntu.com/questions/244406/how-do-i-give-www-data-user-to-a-folder-in-my-home-folder

`usermod -a -G www-data (your username)`

`chgrp www-data /home/myuser/folderA`

`chmod g+rwxs /home/myuser/folderA`



# Ubuntu Desktop install Teamviewer

https://www.linuxbabe.com/ubuntu/install-teamviewer-12-ubuntu-16-04-ubuntu-16-10


# Install .deb

https://www.linuxbabe.com/ubuntu/install-teamviewer-12-ubuntu-16-04-ubuntu-16-10


# Load Balance Apache2
`

  <VirtualHost *:80>
  
        ProxyRequests off

        ServerName domain.com

        <Proxy balancer://mycluster>
                # WebHead1
                BalancerMember http://10.176.42.144:80
                # WebHead2
                BalancerMember http://10.176.42.148:80

                # Security "technically we aren't blocking
                # anyone but this is the place to make
                # those changes.
                Require all granted
                # In this example all requests are allowed.

                # Load Balancer Settings
                # We will be configuring a simple Round
                # Robin style load balancer.  This means
                # that all webheads take an equal share of
                # of the load.
                ProxySet lbmethod=byrequests

        </Proxy>

        # balancer-manager
        # This tool is built into the mod_proxy_balancer
        # module and will allow you to do some simple
        # modifications to the balanced group via a gui
        # web interface.
        <Location /balancer-manager>
                SetHandler balancer-manager

                # I recommend locking this one down to your
                # your office
                Require host example.org

        </Location>

        # Point of Balance
        # This setting will allow to explicitly name the
        # the location in the site that we want to be
        # balanced, in this example we will balance "/"
        # or everything in the site.
        ProxyPass /balancer-manager !
        ProxyPass / balancer://mycluster/

  </VirtualHost>
  
`

## Webmin

https://www.digitalocean.com/community/tutorials/how-to-install-webmin-on-ubuntu-16-04



# Change Hostname

<code>vi /etc/hostname</code>

<code>vi /etc/hosts</code>

# Apache change port

/etc/apache2/ports.conf

<code>Listen 8079</code>

/etc/apache2/sites-enabled/000-default.conf

<code><VirtualHost *: 8079></code>
  
<code>sudo service apache2 restart</code>


# Open port Firewall

`sudo iptables -A INPUT -p tcp --dport 3306 -j ACCEPT`



## link phpmyadmin

`sudo ln -s /usr/share/phpmyadmin /var/www/html`

หรือ

`sudo nano /etc/apache2/apache2.conf`

และเพิ่ม

`Include /etc/phpmyadmin/apache.conf`


### How To Add Swap Space on Ubuntu 16.04

https://www.digitalocean.com/community/tutorials/how-to-add-swap-space-on-ubuntu-16-04


## NVM

https://askubuntu.com/questions/672994/how-to-install-nodejs-4-using-apt



## SuperVisor
https://www.digitalocean.com/community/tutorials/how-to-install-and-manage-supervisor-on-ubuntu-and-debian-vps


```
[program:email-queue]
process_name=%(program_name)s_%(process_num)02d
command=php /var/www/laravel-example/artisan queue:work redis --queue=emailqueue --sleep=3 --tries=3
autostart=true
autorestart=true
user=forge
numprocs=2
redirect_stderr=true
stdout_logfile=/var/www/laravel-example//storage/logs/supervisord.log
```

## UFW
https://www.digitalocean.com/community/tutorials/how-to-set-up-a-firewall-with-ufw-on-ubuntu-14-04

`sudo ufw allow from 15.15.15.51 to any port 22`
`sudo ufw status numbered`
`sudo ufw delete 2`

## Kill process using port
`netstat -vanp tcp | grep 3000`
หรือ ใน MAC
`sudo lsof -i tcp:3000`

`kill -9 1123`


## Multiple lan card ubuntu
https://askubuntu.com/questions/778392/install-second-network-interface-on-virtualized-ubuntu-server

Get the new interface name using `ifconfig -a`

open `/etc/network/interfaces` and add
```
# The secondary network interface
auto enp0s8
iface enp0s8 inet dhcp
```
`sudo service networking restart`

## RSA
https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys-on-ubuntu-1604
