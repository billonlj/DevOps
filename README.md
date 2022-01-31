# DevOps
## Compte rendue 
### Database
**Why should we run the container with a flag -e to give the environment variables?**  
Cela permet plus de sécurité en évitant par exemple de devoir écrire les mots de passe dans un fichier de configuration  

**Why do we need a volume to be attached to our postgres container ?**
Cela nous permets de faire persiter nos données malgrés l'arrets/supression du docker

Built && run database container
```
docker build -t billonlj\postgres_db .
docker run -d -p 5432:5432 --name postgres_db -v /home/billonlj/CPE-Lyon/DevOps/Database/db-data/:/var/lib/postgresql/data billonlj\postgres_db
```
### Backend API

Built && run Backend container
```
docker build -t billonlj\java .
docker run -p 5656:5656 --name java_main billonlj\java
```


## Commande
build une image depuis un Dockerfile : 
```
docker build -t <name_image> 
```

Lancer un conteneur : 
```
docker run <conteneur_name>
```

récuperer une image : 
```
docker pull <image_name>
```

Voir les images disponibles sur la machine
```
docker images
```

Voir les conteneurs actif sur la machine
```
docker ps
```

Voir les conteneurs qui ont été exécuter sur la machine
```
docker ps -a
```
