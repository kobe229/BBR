# BBR For Debian 9

Please note that this script is made and tested on Debian 9 (stretch) only. Other Debian system (e.g. Debian 8 jessie) may work as well but I could not sure. Other linux system including Ubuntu and Cent OS is **NOT Compatible**!

## Install Guide

```
wget https://raw.githubusercontent.com/S8cloud/BBR/master/bbr.sh && bash bbr.sh install
```

**You may need to REBOOT the server and then run `bbe.sh` again to start BBR:**

```
bash bbr.sh start
```

## Check Guide

If you want to know whether BBR runs well on your Debian 9 server, you can use `lsmod | grep tsunami` to check.
Receiving a message like the follow means you can enjoy BBR right now or you may have to run the bash again!

```
## Example Message ##

root@Debian:~# lsmod | grep tsunami
tcp_tsunami            16384  8
```
