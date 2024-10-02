# mullvad

## cmd
```
mullvad-exclude <app>       ... start app excluded from tunnel

mullvad split-tunnel list 
mullvad split-tunnel add <pid>
mullvad split-tunnel delete <pid>
mullvad split-tunnel clear      --- end all exclusion

https://mullvad.net/check
split tunneling > launch app in settings
https://mullvad.net/en/help/split-tunneling-with-the-mullvad-app#linuxapp
$ mullvad-exlucde to launch outside tunnel

mullvad-exclude st&!
split tunneling; launch suckless terminal outside of mullvad vpn to communicate with local net

   https://mullvad.net/en/help/how-use-mullvad-cli#basic-commands

mullvad connect
mullvad status ° check mullvad VPN connection
mullvad account get ° mullvad VPN account info 
mullvad relay list ° list mullvad VPN servers
mullvad relay set location se mma ° set mullvad location [country] [city]
mullvad relay set location se-mma-wg-001     ° specific server
```

## servers
```
lv  rix  Latvia, riga
rs  be   serbia, belgrad
pt  lis  portugal, lisboa
jp  osa  japan, osaka
de  ber  germany, berlin
br  sao  brazil, sao paolo
al  tia  albiana, tirana
pl  waw  poland, warsaw
se  mma  sweden malmö (mullvad owned)
```

## VPN split tunnel
    1. split tunnel <alacritty>
    2. connect <smb> in <alacritty>
    3. run <st> from <dmenu>
    4. check <w3m whatismypublicip.com> in <st>
    5. run <rtorrent> in <st>



