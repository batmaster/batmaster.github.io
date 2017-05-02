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