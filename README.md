### I. Basics
## ☀️ Carte réseau WiFi

adresse MAC de votre carte WiFi: 28-6B-35-F0-78-A0
adresse IP de votre carte WiFi:10.33.79.155
masque sous reseau LAN: 255.255.240.0 (CIDR /20)

## Déso pas déso
l'adresse de réseau du LAN auquel vous êtes connectés en WiFi:10.33.64.0
l'adresse de broadcast:10.33.79.255
le nombre d'adresses IP disponibles dans ce réseau:4094

### ️ Hostname

Hostname : DESKTOP-BJE98E8

###  Passerelle du réseau
IP passerelle : 10.33.79.254
MAC passerelle :7c-5a-1c-d3-d8-76

### Serveur DHCP et DNS

serveur DHCP :  10.33.79.254
serveur DNS : 8.8.8.8 et 1.1.1.1

###  Table de routage
table de routage: Destination réseau    Masque réseau  Adr. passerelle   Adr. interface Métrique
          0.0.0.0          0.0.0.0     10.33.79.254     10.33.79.155     30

### II. Go further

## ️ Hosts ?


PS C:\Users\T> ping b2.hello.vous

Envoi d’une requête 'ping' sur b2.hello.vous [1.1.1.1] avec 32 octets de données :
Réponse de 1.1.1.1 : octets=32 temps=15 ms TTL=55

## Go mater une vidéo youtube et déterminer, pendant qu'elle tourne...

l'adresse IP du serveur auquel vous êtes connectés pour regarder la vidéo: 91.68.245.17
le port du serveur auquel vous êtes connectés:443
le port que votre PC a ouvert en local pour se connecter au port du serveur distant: 64486

## Requêtes DNS
PS C:\Users\T> nslookup www.thinkerview.com
>>
Serveur :   dns.google
Address:  8.8.8.8

Réponse ne faisant pas autorité :
Nom :    www.thinkerview.com
Addresses:  2a06:98c1:3120::7
          2a06:98c1:3121::7
          188.114.96.7
          188.114.97.7

PS C:\Users\T> nslookup 143.90.88.12
>>
Serveur :   dns.google
Address:  8.8.8.8

Nom :    EAOcf-140p12.ppp15.odn.ne.jp
Address:  143.90.88.12

##  Hop hop hop

PS C:\Users\T> tracert www.ynov.com
>>

Détermination de l’itinéraire vers www.ynov.com [172.67.74.226]
avec un maximum de 30 sauts :

  1     6 ms     1 ms     1 ms  10.33.79.254
  2     2 ms     1 ms     2 ms  145.117.7.195.rev.sfr.net [195.7.117.145]
  3     3 ms     3 ms     2 ms  237.195.79.86.rev.sfr.net [86.79.195.237]
  4     4 ms     3 ms     3 ms  196.224.65.86.rev.sfr.net [86.65.224.196]
  5    13 ms    11 ms    60 ms  164.147.6.194.rev.sfr.net [194.6.147.164]
  6     *        *       17 ms  162.158.20.24
  7    16 ms    16 ms    16 ms

## IP publique

  195.7.117.146


### III. Le requin

![image wireshark](C:\Users\T\Downloads\arp.pcapng)