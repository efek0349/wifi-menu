# OpenBSD Wireless Network Management Script

Usage :
	$ doas ./wifi-menu <interface\>
```
   .;'                     `;,            
  .;'  ,;'             `;,  `;,    OpenBSD Wireless Network Management Script
 .;'  ,;'  ,;'     `;,  `;,  `;,   OS      :OpenBSD 7.6 amd64
 ::   ::   :   ( )   :   ::   ::   SHELL   :ksh   
 ':.  ':.  ':. /_\ ,:'  ,:'  ,:'   TERM    :rxvt-256color  
  ':.  ':.    /___\    ,:'  ,:'    PC      :LENOVO 20KN007
   ':.       /_____\      ,:'     
            /       \     

1) Normal.iwm0         2) Test.iwm0             7) Raspi3.iwm0
2) Privacy.iwm0        3) Android.iwm0
3) MyVPN.iwm0          4) CryptoLab.iwm0

[+] Choose a previously saved wifi connection or "Enter" to skip:
1) Android1        4) Wifi4          7) Wifi7
2) Wifi2           5) Wifi5
3) Wifi3           6) Wifi6

[+] Choose wifi connection or "Enter" to quit: 1
[+] Enter the passphrase for "Android1"?
[+] Password:
[+] Creating new configuration using "Android1"
[+] Connecting using file "Android1"
[+] Configured interface iwm0; ESSID is "Android1"
[+] Interface iwm0 is up
[+] Running dhcpleasectl
....
iwm0 [Bound]
	inet 192.168.1.104 netmask 255.255.255.0
	default gateway 192.168.1.1
	lease 24 hours
	dhcp server 192.168.1.1
dnscrypt_proxy(ok)
dnscrypt_proxy(ok)
unbound(ok)
unbound(ok)
```

# alias

### alias conn-cryptolab='printf "4\n"| wifi-menu'

```
$ printf "4\n"| doas /usr/local/bin/wifi-menu iwm0
   .;'                     `;,
  .;'  ,;'             `;,  `;,    OpenBSD Wireless Network Management Script
 .;'  ,;'  ,;'     `;,  `;,  `;,   OS      :OpenBSD 7.6 amd64
 ::   ::   :   ( )   :   ::   ::   SHELL   :ksh
 ':.  ':.  ':. /_\ ,:'  ,:'  ,:'   TERM    :rxvt-256color
  ':.  ':.    /___\    ,:'  ,:'    PC      :LENOVO 20KN007UTX
   ':.       /_____\      ,:'
            /       \

1) Normal.iwm0         2) Test.iwm0             7) Raspi3.iwm0
2) Privacy.iwm0        3) Android.iwm0
3) MyVPN.iwm0          4) CryptoLab.iwm0

[+] Select a previously saved WiFi connection or press "Enter" to skip:
[+] "CryptoLab.iwm 0" is selected
[+] Connecting using the "CryptoLab.iwm0" configuration file.
[+] Interface iwm0 has been configured the ESSID is "CryptoLab.iwm0"
[+] Interface iwm0 is now up
[+] Running dhcpleasectl
......
iwm0 [Bound]
	inet 192.168.1.137 netmask 255.255.255.0
	default gateway 192.168.1.1
	lease 24 hours
	dhcp server 192.168.1.1
dnscrypt_proxy(ok)
dnscrypt_proxy(ok)
unbound(ok)
unbound(ok)
```
