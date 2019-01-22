Rpi_Zram
Script to enable ZRAM on a Raspberry Pi.

Automatically detects the number of CPU cores to allocate to ZRAM computation, disables existing swap and enables ZRAM swap.

Download the script and copy to /usr/bin/ folder

sudo wget -O /usr/bin/zram.sh https://github.com/ElectrooPi/Zram/Zram,sh

make file executable

sudo chmod +x /usr/bin/zram.sh

edit /etc/rc.local file to run script on boot

sudo nano /etc/rc.local

add line before exit 0

/usr/bin/zram.sh &
