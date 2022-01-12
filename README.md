
*Ce workshop à pour but de vous expliquer ce que sont les outils **Docker** et **Docker-compose** et comment les utiliser dans vos projets ou pour déployer des conteneurs Docker*

**N'hésitez pas à star ⭐ le repo si vous avez aimé ce workshop!**

![](https://img.shields.io/github/stars/ajnart/workshop-docker?label=%E2%AD%90&style=for-the-badge?branch=master&kill_cache=1")

# Introduction
## Docker
![](assets/docker_logo.svg)

### Qu'est-ce que Docker ?

**Docker** est une plateforme de conteneurs lancée en 2013 ayant largement contribué à la démocratisation de la conteneurisation. Elle permet de créer facilement des conteneurs et des applications basées sur les conteneurs. Il en existe d’autres, mais celle-ci est la plus utilisée.

### Conteneur ?
Un contenur est une sorte de boîte dans laquelle une version minimisée d'un OS est installée, permettant l'execution d'un programme ou d'un service spécifique sur n'importe quel OS*(ex: Apache, MySQL, PHP, etc...)*

Source: https://www.docker.com/resources/what-container


### Pourquoi Docker ?
Dockeriser un projet est une bonne idée car il permet de séparer les ressources de votre projet, de faciliter le déploiement et de faciliter la maintenance. Il n'y aura donc pas de problème de déploiement si vous changez de machine, il faudra seulement Docker Engine.

## Docker-compose
![](assets/compose_logo.svg)

### Qu'est-ce que Docker-compose ?
Docker Compose est un outil qui permet de décrire *(dans un fichier YAML)* et gérer *(en ligne de commande)* plusieurs conteneurs comme un ensemble de services inter-connectés.  
Compose créer un *réseau virtuel* qui permet aux services de communiquer simplement entre eux.  

# Déroulement du workshop
- 1 : Installation de docker et docker-compose
- 2 : Hello World!
- 3 : Docker-compose 

## Installation de docker et docker-compose
Suivez les instructions ci-dessous pour installer Docker et Docker-compose sur votre machine:  
https://docs.docker.com/get-docker/  
⚠ Si vous êtes sur Linux, faites bien les étapes [post-install](https://docs.docker.com/engine/install/linux-postinstall/) avant de continuer. Cela permettra de lancer Docker sans avoir à entrer votre mot de passe root avec ``sudo`` ou ``doas``.
⚠ Il n'est pas nécessaire d'installer Docker desktop. 

## Hello World!
Suivez les instructions ci-dessous pour créer le conteneur "Hello world" de Docker: https://hub.docker.com/_/hello-world  
``docker run hello-world``  
Si un message d'erreur apparait, vérifiez que vous avez bien installé Docker et Docker-compose.
## Docker-compose
Suivez les instructions [getting started with docker compose](https://docs.docker.com/compose/gettingstarted/) pour créer une stack contenant Python Flask (serveur HTTP) et Redis (Base de données)

ensuite, vous devriez pourvoir le lancer avec ``docker-compose up -d``
(-d : démarrer les services en arrière plan, *detached mode*)
⚠ Notez que le code est déjà présent dans ./app

# Conclusion
Merci d'avoir suivi ce workshop ! J'espère qu'il vous à plu.  
Il a pour but de vous familiariser avec Docker et compose pour vous préparer aux autres workshops que je présente (workshops MyNetflix) dans lesquels Docker et Docker-compose sont utilisés afin de deployer une stack de services permettant le téléchargement, gestion et l'automatisation de médias. (séries, films, musiques, etc...)
