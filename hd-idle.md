# hd-idle

spin down hdd timeout

## documentation
- [docu](https://thudak.com/blog/2019-01-24-spin-down-hdd-with-raspberry-pi-using-hd-idle/)
- [for raspberry](https://superuser.com/questions/651880/force-spin-down-of-external-hard-drive-on-linux-raspberry-pi)

## cmd
```
sudo nano /etc/default/hd-idle                                     
HD_IDLE_OPTS="-i 600 -a /dev/sda"                                  
sudo systemctl restart hd-idle                                     
```


