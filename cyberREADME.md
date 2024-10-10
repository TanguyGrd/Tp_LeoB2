## Clients du réseau
Adresse IP	Nom d'hôte	Adresse MAC	Fabricant
192.168.1.56	DESKTOP-IUKA3LU.lan	04:D4:C4:D3:4D
	ASUSTek Computer
192.168.1.135	Bouygtel4K-272011121428054.lan	EC:6C:9A:DD:F9:9E	Arcadyan
192.168.1.254	bbox.lan	30:93:BC:88:4B:6C	Sagemcom Broadband SAS
192.168.1.9	host.docker.internal	N/A	N/A
 ## Équipements fixes

    Routeur : bbox.lan (192.168.1.254)
    PC : DESKTOP-IUKA3LU (192.168.1.56)
        Ports ouverts : 80 (HTTP), 902 (VMware Authentication), 912 (VMware Authentication), 3306 (MySQL), 5357 (HTTPAPI)

# Bornes Wi-Fi

    Pour obtenir la liste des points d'accès Wi-Fi visibles, utilise la commande suivante :

    "netsh wlan show networks mode=bssid"

## Switches
Appareils identifiés

    DESKTOP-IUKA3LU.lan
        Adresse IP: 192.168.1.56
        Adresse MAC: 04:D4:C4:D3:4D
        Fabricant: ASUSTek Computer

    Bouygtel4K-272011121428054.lan
        Adresse IP: 192.168.1.135
        Adresse MAC: EC:6C:9A:DD:F9:9E
        Fabricant: Arcadyan

    Galaxy-A12.lan
        Adresse IP: 192.168.1.194
        Adresse MAC: DE:F3:08:FF:6D:81
        Fabricant: Inconnu

    bbox.lan
        Adresse IP: 192.168.1.254
        Adresse MAC: 30:93:BC:88:4B:6C
        Fabricant: Sagemcom Broadband SAS (probablement un routeur)

    host.docker.internal
        Adresse IP: 192.168.1.9
        Adresse MAC: 00:00:00:00:00:00 (adresse réservée pour Docker)

Vérifier avec MAC Vendor

## Ports RJ45

    Tests effectués sur la plage d'adresses IP 192.168.1.100-150 :

    "nmap -sn 192.168.1.100-150"

Résultats du scan

    Appareil détecté :
        Nom d'hôte : Bouygtel4K-272011121428054.lan
        Adresse IP: 192.168.1.135
        Adresse MAC: EC:6C:9A:DD:F9:9E
        Fabricant: Arcadyan

Emplacement de la salle serveur
(fait depuis chez moi donc j'en ai pas)

## Risques potentiels

Services ouverts non sécurisés identifiés sur DESKTOP-IUKA3LU :

"Considérer des mesures de sécurité pour protéger ces services, notamment la configuration de pare-feu et la restriction d'accès." 

(Ports ouverts :
    80 (HTTP) : Utilisé pour le trafic web non sécurisé. Sans HTTPS, il peut être vulnérable aux attaques de type "man-in-the-middle".
    3306 (MySQL) : Utilisé pour accéder aux bases de données MySQL. S'il est accessible depuis l'extérieur du réseau local, cela peut représenter une menace.
    902 et 912 (VMware) : Ces ports sont utilisés pour des services de virtualisation. Si mal configurés, ils peuvent exposer des vulnérabilités.
    5357 (HTTPAPI) : Utilisé pour des services de découverte de périphériques. Une mauvaise configuration peut également poser des problèmes de sécurité.)