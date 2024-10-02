# System

General hints for (manjaro) Linux

## ssh
```
    disable last login message on ssh connection
    touch ~/.hushlogin

    ssh-keygen  generate local keyfile
    ssh-copy-id user@host   copy keyfile to ssh server
    sshpass automates password login
    sshpass -p xxxxx ssh user@192.168.178.171°ssh raspberry home
```

## file locations
```
login delay after fail attempts https://askubuntu.com/questions/877385/how-can-i-lower-the-delay-after-incorrectly-entered-login-and-sudo-passwords
sudo update-rc.d ssh enable/remove      (don't) start service on boot
sudo vim /etc/rc.local      scripts at startup
sudo password delay https://unix.stackexchange.com/questions/40954/how-does-one-change-the-delay-that-occurs-after-entering-an-incorrect-password 
.fzf.bash       ... list of ** completion progs
.xinitrc ... wm + ressources
snap mount cmds in /etc/systemd/system
/var/lib/pacman/
/var/cache/pacman/pkg       heruntergeladene pacman pakete zur Installation; auch nach kopmpilierung
   .fzf.bash        bash completion rules for **
/home/xaos/.local/share/applications/dropbox.desktop		# desktop entries
cat /proc/asound/cards		# sound devices

.desktop categories	https://unix.stackexchange.com/questions/177212/add-new-category-to-applications

.desktop files go in /.local/share/applications/sxiv.desktop

mailto links handled by mailto.desktop (via x-scheme in mimeapps.list)


alternatives askpass /usr/lib/ssh/askpass   (from package x11-ssh-askpass)
    docu:	https://man.archlinux.org/man/x11-ssh-askpass.1x
        https://github.com/sigmavirus24/x11-ssh-askpass/blob/master/SshAskpass-1337.ad
    Problem mit Umlauten
    configuration Ã¼ber makefile; kein .conf

run GUIs as root
    https://unix.stackexchange.com/questions/254072/how-do-i-ask-password-by-gui-prompt-while-using-sudo-in-script
    
    install nps-ssh-askpass via snapp		https://sourceforge.net/projects/nps-ssh-askpass/
    edit /etc/sudo.conf
        # add Path to askpass helper program for sudo -A
        Path askpass /var/lib/snapd/snap/bin/nps-ssh-askpass
    call sudo -A command
    
    support nps-ssh-askpass	https://snapcraft.io/nps-ssh-askpass
    
notify-send design: .dunstrc
export PATH=/home/dave/work:$PATH

$HOME
$PWD
$BROWSER
$EDITOR
$MAIL
$PATH
bspw. export EDITOR=vim
etc/pacman.d/mirrorlist
.config/user-dirs.dirs
/etc/fstab	automount table
change background login screen	/etc/lightdm/lightdm-gtk-greeter.conf

## Grub
sudo grub-mkconfig -o /boot/grub/grub.cfg
sudo update-grub

/etc/default/grub editieren und anschließend: "sudo update-grub" 
backlight: edited grub boot line ... acpi_backlight=native + /etc/X11/xorg.conf
https://wiki.archlinux.org/title/backlight
https://askubuntu.com/questions/715306/xbacklight-no-outputs-have-backlight-property-no-sys-class-backlight-folder
[grub] 'e' to edit boot menu
repair steps
EFI variablen mit einbinden! https://unix.stackexchange.com/questions/91620/efi-variables-are-not-supported-on-this-system
for i in /dev /dev/pts /proc /sys /sys/firmware/efi/efivars /run; do sudo mount -B $i /mnt$i; done
https://wiki.manjaro.org/index.php/GRUB/Restore_the_GRUB_Bootloader
https://forum.manjaro.org/t/reinstall-grub2/27477/6
https://www.shellhacks.com/reinstall-grub-from-live-usb-uefi-lvm/
https://askubuntu.com/questions/740253/how-to-install-grub-in-an-external-hard-drive
https://askubuntu.com/questions/737319/ubuntu-is-booting-very-slowly-after-dual-boot-with-kali/737340#737340
```

## Encryption
```
    encrypt dir

    veracrypt command line
    https://veracrypt.eu/en/Command%20Line%20Usage.html
    veracrypt -t  /mnt/archiv-ckw/Unterlagen.hc /mnt/archiv-unterlagen
    t
    gpg
    gpg-zip

    openssl des3 -salt -in unencrypted-data.tar -out encrypted-data.tar.des3
    openssl des3 -d -salt -in encrypted-data.tar.des3 -out unencrypted-data.tar

    aescrypt -e -p password file.jpg
    aescrypt -d -p password file.jpg.aes

    Open Encrypted Directory:
    openssl enc -aes-256-cbc -d -in ~/vault.tar.gz.dat | tar xz; thunar ~/vault

    Lock Encrypted Directory:
    tar cz vault/ | openssl enc -aes-256-cbc -out ~/vault.tar.gz.dat; rm -r ~/vault
```

## SSH -X
```
ssh control remote terminal displayed on remite machine
    ssh -X      X forwarding
    ssh -Y display remote programs locally
    https://superuser.com/questions/123765/how-can-i-run-a-program-remotely-via-ssh-but-display-locally

    https://unix.stackexchange.com/questions/12755/how-to-forward-x-over-ssh-to-run-graphics-applications-remotely
```

## superuser defaults
```
    sudo visudo
    Defaults        passwd_timeout=0 # time the password promt remains
    Defaults        timestamp_timeout=15 # time the sudo command lasts
```

