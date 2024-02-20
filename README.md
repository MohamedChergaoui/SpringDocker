# SpringDocker
Introduction à Dockerfile
Le Dockerfile est un fichier texte qui contient les instructions nécessaires pour créer une image Docker. Il définit l'environnement d'exécution de l'application et les dépendances requises.

Création du Dockerfile
Ouvrez un éditeur de texte et créez un nouveau fichier nommé Dockerfile à la racine de votre projet.

Utilisez des instructions Dockerfile telles que FROM, COPY, RUN, EXPOSE, et CMD pour définir les étapes de construction de l'image Docker. Exemple :
<img width="736" alt="Capture d’écran 2024-02-20 à 15 46 11" src="https://github.com/MohamedChergaoui/SpringDocker/assets/61020088/05353867-d0a8-4800-93fe-59094a4f4215">



#Ajoutez une section dans votre Dockerfile pour inclure PostgreSQL. Utilisez une image officielle de PostgreSQL depuis Docker Hub.

Construction de l'Image Docker
Ouvrez un terminal et accédez au répertoire contenant votre projet Spring Boot et le Dockerfile.

Exécutez la commande suivante pour construire l'image Docker :
*/ docker build -t Lab_exprt .

 cmd2 : pou cree un contenaire Postgres.
  docker run --name postgres-bases -e POSTGRES_PASSWORD=yasso -p 8000:5432 -d postgres
cmd3 : image pour le project docker 
  docker build -t myapp
cmd4: create network
  docker network create new-network-labnetwork
cmd5: créer et exécuter un nouveau conteneur Docker basé
docker run --name create new-network-labnetwork
docker run --name postgres-bases --network new-labnetwork
