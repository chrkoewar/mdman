# mount

```
mount can handle .iso
mount home to other partition
https://www.howtogeek.com/442101/how-to-move-your-linux-home-directory-to-another-hard-drive/

mount mit schreibrechten für nutzer:
sudo mount -o uid=1000 /dev/sdb1 ~/media/usb
https://superuser.com/questions/320415/mount-device-with-specific-user-rights

automount
sudo mount -t ntfs-3g -o rw /dev/sda4/ media/data
mount -t ntfs-3g -o rw /dev/sda1 /root/win  
add to /etc/fstab: UUID=DEE26575E2655337     /media/data ntfs-3g    defaults    0   0
wichtig: https://askubuntu.com/questions/34731/howto-auto-mount-windows-partitions-using-etc-fstab

mount usb drive
fdisk -l > liste
mount /dev/sdb1 /media/usb 
setgid https://wiki.ubuntuusers.de/Windows-Partitionen_einbinden/NTFS-3G/
```

