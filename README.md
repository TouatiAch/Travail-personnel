# Travail-personnel

Exercice 1 :
Commandes exécutées :
+ Pour créer l'image docker : docker build -t ubuntu-ping .
+ Pour lancer le conteneur : docker run -it ubuntu-ping
+ Pour Tester : ping 8.8.8.8

Exercice 2 :
Commandes exécutées :
+ Pour créer l'image docker : docker build -t ubuntu-ssh .
+ Pour lancer deux conteneurs : docker run -d --name conteneur1 ubuntu-ssh
                                docker run -d --name conteneur2 ubuntu-ssh
+ Trouver l'adresse IP de conteneur2 : docker inspect -f '{{range.NetworkSettings.Networks}}{{.IPAddress}}{{end}}' conteneur2
+ Se connecter en SSH depuis conteneur1 : ssh root@172.17.0.3

Exercice 3 :
Commandes exécutées :
+ Pour créer l'image docker : docker build -t apache-server .
+ Pour lancer le conteneur :  docker run -d -p 8080:80 apache-server

Exercice 4 :
Commandes exécutées :
+ Pour lancer les services avec docker compose : docker-compose up -d





