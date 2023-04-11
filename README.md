# ReseauProjet

Nous avons pas utilisé GIT pour le projet mais voici les traces que nous avons utilisé.

Pour effectuer nos différentes analyse, nous avons appliquer des filtres globaux afin d'isoler l'application zoom  

Rem: nous avons utilisé linux pour que le traffic soit plus restreint

commande : 

```
nestat -np --inet | grep zoom
```

Exemple de connexion établie :

```
tcp        0      0 192.168.182.72:43988    206.247.69.16:443       ESTABLISHED 4521/zoom           
tcp        0      0 192.168.182.72:43020    170.114.11.104:443      ESTABLISHED 4521/zoom           
tcp        0      0 192.168.182.72:43994    206.247.69.16:443       ESTABLISHED 4521/zoom           
tcp        0      0 192.168.182.72:43986    206.247.69.16:443       ESTABLISHED 4521/zoom           
tcp        0      0 192.168.182.72:44000    206.247.69.16:443       ESTABLISHED 4521/zoom           
tcp        0      0 192.168.182.72:38326    170.114.52.5:443        ESTABLISHED 4521/zoom           
tcp        0      0 192.168.182.72:45080    170.114.15.194:443      ESTABLISHED 4521/zoom           
tcp        0      0 192.168.182.72:44024    206.247.69.16:443       ESTABLISHED 4521/zoom           
tcp        0      0 192.168.182.72:44008    206.247.69.16:443       ESTABLISHED 4521/zoom           
tcp        0      0 192.168.182.72:44028    206.247.69.16:443       ESTABLISHED 4521/zoom           
tcp        0      0 192.168.182.72:33118    170.114.14.62:443       ESTABLISHED 4521/zoom           

ip.addr == 206.247.69.16 or ip.addr == 170.114.11.104 or ip.addr == 170.114.52.5 or ip.addr == 170.114.15.194 or ip.addr == 170.114.14.62
```
