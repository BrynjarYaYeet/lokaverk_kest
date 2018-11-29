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
## Fyrirtæki
>

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
> Stillti Ip address(192.168.25.2) á g0/0(Tengist í S_FIBER) hjá R_ISP.
