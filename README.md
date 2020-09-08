# PING
Ce projet consiste à recoder la commande ping.

## RESUME
Ping est le nom d’une commande informatique permettant de tester l’accessibilité
d’une autre machine à travers un réseau IP. La commande mesure également le temps
mis pour recevoir une réponse, appelé round-trip time (temps aller-retour).
Mike Muuss a écrit ce programme en décembre 1983 pour déboguer un comportement
anormal sur réseau IP. Le nom est tiré de l’onomatopée décrivant le son émis par un
sonar puisque leur action est similaire (émission d’un signal qui vient rebondir sur une
cible pour revenir à l’envoyeur).
Par la suite, David L. Mills a fourni un rétro-acronyme : « Packet InterNet Groper ».

## BEHAVIOUR
```sh
gbourgeo@debian:~/Work/ping$ ./ft_ping 
Usage: ft_ping [-nqvh] [-c count] [-s packetsize] [-t ttl] destination
  -c <count>
    Stop after sending count ECHO_REQUEST packets. With deadline option, ping waits for count
    ECHO_REPLY packets, until the timeout expires.
  -h
    Show help.
  -n
    Numeric output only.  No attempt will be made to lookup symbolic names for host addresses.
  -q
    Quiet output.  Nothing is displayed except the summary lines at startup time and when finished.
  -s <packetsize>
    Specifies the number of data bytes to be sent. The default is 56, which translates into 64 ICMP
    data bytes when combined with the 8 bytes of ICMP header data.
  -t <ttl> ping only.
    Set the IP Time to Live.
  -v
    Verbose output.

```
+ Gestion d'une IPv4 simple (adresse/hostname) comme paramètre du programme.
+ Gestion du FQDN sans pour autant effectuer la résolution DNS dans le retour du paquet.

## AUTHOR
+ Gilles BOURGEOIS
