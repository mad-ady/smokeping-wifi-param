# smokeping-wifi-param
Probe to extract wifi parameters of a wifi card with smokeping

Installation:
```
 wget https://raw.githubusercontent.com/mad-ady/smokeping-wifi-param/master/WifiParam.pm -O /usr/share/perl5/Smokeping/probes/WifiParam.pm
 ```
 
 Configuration:
``` 
+ WifiParam
binary = /sbin/iw
pings = 3
step = 300
offset = random

++ WifiParamsWlan0
interface = wlan0

+++ WifiParamsWlan0Freq
parameter = freq

+++ WifiParamsWlan0Signal
parameter = signal

+++ WifiParamsWlan0Bitrate
parameter = bitrate

++ WifiParamsWlan1
interface = wlan1

+++ WifiParamsWlan1Freq
parameter = freq

+++ WifiParamsWlan1Signal
parameter = signal

+++ WifiParamsWlan1Bitrate
parameter = bitrate
```
