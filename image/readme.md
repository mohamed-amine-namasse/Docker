Vérifier la version d'installation de docker avec la commande:
docker --version
![alt text](image.png)
Test des commandes de bases:
docker info
![alt text](image-1.png)
![alt text](image-2.png)
![alt text](image-3.png)

docker ps
![alt text](image-4.png)

docker images
![alt text](image-5.png)

docker run
![alt text](image-6.png)

docker run -d --name mon-web-serveur -p 80:80 nginx
![alt text](image-7.png)

docker stop
![alt text](image-8.png)
docker stop mon-web-serveur
![alt text](image-9.png)

Récupérer l’image Docker:

docker pull
![alt text](image-10.png)
docker images
![alt text](image-11.png)
Construction du container Docker
docker run -it --rm -p 8080:80 docker/welcome-to-docker
![alt text](image-12.png)
![alt text](image-13.png)
docker run -it -d --rm -p 8080:80 docker/welcome-to-docker
![alt text](image-14.png)

Arréter le conteneur
On fait docker ps pour lister les conteneurs
![alt text](image-15.png)
On arrete le conteneur a travers son nom ou ID avec docker stop id/nom et on reliste tous les conteneurs avec docker ps-a (-a pour all), on voit bien qu'on a plus de conteneur
![alt text](image-16.png)
