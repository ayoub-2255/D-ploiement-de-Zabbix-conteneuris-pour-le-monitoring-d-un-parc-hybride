1-Présentation du projet

Ce projet consiste à concevoir et déployer une infrastructure cloud de supervision centralisée sur AWS, permettant de surveiller en temps réel des machines Linux et Windows.

La solution repose sur :

AWS EC2 pour l’hébergement

Docker & Docker Compose pour le déploiement du serveur Zabbix

Zabbix Agent pour la collecte des métriques système



2-Composants : 

1 serveur Zabbix (Dockerisé)

1 client Linux (Ubuntu)

1 client Windows (Windows Server)

<img width="1860" height="477" alt="les 3 instances créer " src="https://github.com/user-attachments/assets/6a7438e4-ba8e-43c3-be59-7d6fad5340dc" />


3- Zabbix

Toutes les instances sont déployées dans un VPC AWS, avec communication via IP privées.

Le serveur Zabbix est déployé à l’aide de Docker Compose.

<img width="1257" height="1000" alt="docker compoose avec mariadb" src="https://github.com/user-attachments/assets/3a389cc2-e7c4-4063-bedc-2f61a0897bf1" />

docker-compose up -d

on obtient alors le dashboard zabbix 

<img width="1879" height="922" alt="dashboard zabix" src="https://github.com/user-attachments/assets/86475048-be0a-4550-ad4e-dcf8554b201b" />


<img width="1868" height="841" alt="les 3 client marchent" src="https://github.com/user-attachments/assets/2fa852c4-51ed-4421-875f-5ab95d862ce3" />


