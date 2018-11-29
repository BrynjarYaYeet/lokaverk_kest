# lokaverk_kest

# 22 Nóv 2018
## Heimanet
> Stilti heimanetinu upp. 
> Tengdi borðtölvu og prentara við router með copper straight-through.
> Setti upp gesta wifi þar sem Network name: Gestanet, Security mode: WPA2 Personal, Encryption: AES og Passphrase: gestur123.
> Setti upp venjulegt wifi þar sem Network name: Heimanet, Security mode: WPA2 Personal, Encryption: AES og Passphrase: Password.
> Tengdi Svein, Íþróttaálfinn, Halla og Margréti við heimanet.
> Tengdi Lárus við gestanetið.

## Fyrirtæki
> Stilti fyrirtækjanetinu upp.
> Tengdi switch0 við routerinn.
> Tengdi pc1 - pc8 við switch0.
> Setti upp wifi þar sem Network name: FyrirtækiNet, Security mode: WPA2 Personal, Encryption: AES og Passphrase: Fyrirtaeki.
> Tengdi Gunnar, Jolla, Siggu og Árna við FyrirtækiNet.
> Setti upp gestanet fyrir fyrirtækið þar sem Network name: FyrirtækiGestur, Security mode: WPA2 Personal, Encryption: AES og .Passphrase: FyrirtaekiG.

# 27 Nóv 2018
## Fyrirtæki
> Tengdi PC1 við switchin með blárri snúru.
> Breytti hostname í S_Fyrirtaeki.
> Stillti lykilorð með line(con og vty) og enable secret Password:fyrirtaeki.
> Encryptaði öll lykilorð.
> Setti Banner motd í "Thad er bannad ad stela!!".
> Vlan ip address: 192.168.2.2 255.255.255.0.
> Copy-aði running config í startup config.
> Stillti ip address á routernum í 192.168.2.1 255.255.255.0.
> SSH Domain name: cisco.com, generate rsa, 1024 bita, username admin secret: fyrirtaeki.

## Heimanet
> Stillti ip address á roudernum í 192.168.1.1 255.255.255.0.
> Notaði dhcp til að fá ip tölur á allt á Heimili.

# 29 Nóv 2018
## ISP
> Stilti öllu upp.
> Breytti Hostname á R_ISP í R_ISP.
> Stillti lykilorð á R_ISP og encryptaði Lykilorð=ISP.
> Breytti hostname á Ljósleiðarabox í Ljosleidari.
> Stillti lykilorð á Ljósleiðarabox og encryptaði Lykilorð=ISP.
> Tengdi mig inná RIX með blárri snúru.
> Breytti hostname á RIX í RIX.
> Stillti lykilorð á RIX og encryptaði Lykilorð=RIX123.
> Tengdi mig inná S_FIBER með blárri snúru.
> Breytti hostname á S_FIBER í FIBER.
> Stillti lykilorð á FIBER og encryptaði Lykilorð=FIBER123.
> Tengdi mig inná S_ADSL með blárri snúru.
> Breytti hostname á S_ADSL í ADSL.
> Stillti lykilorð á ADSL og encryptaði Lykilorð=ADSL123.
> Stillti Ip address(192.168.21.10) á g0/0(Tengist í S_FIBER) hjá R_ISP.
> Stillti Ip address(192.168.20.5) á g0/1(Tengist í S_ADSL) hjá R_ISP.
> Stillti Ip address(192.168.23.15) á g0/2(Tengist í RIX) hjá R_ISP.
> Stillti Ip address(192.168.30.2) á fa0/0(Tengist í S_FIBER) hjá Ljósleiðarabox.
> Stillti Ip address(163.85.100.251) á g1/0(Tengist í FyrirtækjaRouter) hjá Ljósleiðarabox.
> Setti upp 2 dns server www.ha.com og ha.com Ip address (á báðum): 150.25.10.5.
> Setti upp DHCP server í gegnum ISP_DHCP(ADSL) þar sem Pool name: DHCP, Deafult gateway: 192.168.20.5, DNS: 150.25.10.5, Start ip: 192.168.20.10, Subnet mask: 255.255.255.0 og Max number of users: 150.
> Breytti ip address á DHCP servernum í 192.168.20.7 255.255.255.0
