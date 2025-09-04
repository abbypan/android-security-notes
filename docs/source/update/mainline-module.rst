Mainline modules (apex/apk)
-------------------------------------------

Mainline module: 可通过google play store独立升级的module，不用走ota

intall dir: /data/app/

开机时可安全校验并使用/data/app下较新版本的module，而非system partition下的旧版module

APEX & APK
-------------

APEX mainline module 针对 system core lib 

APK mainline module 针对 system service


pub key
---------

apex pub key: /system/apex/apexkeys.txt

apk pub key: /system/etc/security/otacerts.zip


pub key owner
------------------

除google mainline module之外，oem也可以发布自身的mainline module

对应不同的pub key





