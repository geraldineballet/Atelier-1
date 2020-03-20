Atelier 1 - 20 03 2020

CAPTURE 1

**1/ Veuillez iden,fier votre serveur GNS3 qui est capgchambX.goffinet.net où X est le numéro de votre serveur.
Pouvez-vous interpréter de la manière la plus précise la commande suivante adaptée de la valeur X de votre serveur ? Quel résultat
fournit-elle ? curl http://capgchamb0.goffinet.net:8003**
Mon serveur GNS3 : capgchamb2.goffinet.net
La commande curl http://capgchamb0.goffinet.net:8003 me donne le nom et l’IP de l’ordinateur :
Name : capgchamb2.goffinet.net
IPv4 : 163.172.178.20


**2/ Veuillez capturer le trafic de ce1e commande uniquement et l'enregistrer sous le nom capture1.pcapng**
Cf. Capture1

**3/ Quel est le numéro du port source u2lisé par le client pour joindre ce6e ressource Internet ?**
Le numéro du port source utilisé est le 8003

**4/ Quel est le numéro du paquet qui con5ent la commande de couche Applica5on ?**
Le paquet 21 contient le protocole http de la couche Application

**5/ Quel est le paquet qui commence la session ? Quel est le paquet qui termine la session ?**
Le paquet 18 commence la session [SYN] ; le paquet 29 termine la session [ACK]. On remarque qu’il y a bien SYN ; SYN ACK ; ACK.



CAPTURE 2

**1/ Pouvez-vous interpréter de la manière la plus précise la commande suivante ? Quel résultat fournit-elle et comment ? dig @ns1.google.com -t TXT o-o.myaddr.l.google.com +short -4**
La commande dig interroge les serveurs DNS pour que l’on puisse voir s’il y a des dysfonctionnements dans la résolution de nom.
La commande dig nous donne l’adresse IP uniquement contrairement à la commande curl de la 1ère capture. 
Elle donne la même IP 163.172.178.20 dans la commande.

**2/ Veuillez capturer le trafic de ce1e commande uniquement et l'enregistrer sous le nom capture2.pcapng.**
Cf. Capture2

**3/ Combien de transactions sont-elles générées ? Pourquoi y en at-il autant ?**
4 transactions DNS, 2 fois 2 transactions "standard query / standard query reponse"
et 2 transactions ARP

Il y en a plusieurs car on interroge le serveur. Ils donnent les différentes possibilité.il faut la question et la réponse à chaque fois.

**4/ Pour chacune des transactions, quelle est la question (QUERY) qui est posée ?**


**5/ Pour chacune des transactions, à quel ordinateur est posée la question ?**




