# DevOps
## Commande

Lancer un conteneur : 
```
docker run <conteneur_name>
```
Option :  
-**i** Garder STDIN ouvert, même si pas attaché  
-**t** Allouer un pseudo-terminal  
-**p** Permet de publier un conteneur, et accessible via une translation de port depuis le serveur.  
-**d** Active le mode daemon. Le conteneur sera actif et en tâche de fond  
-**e** Force Docker a utiliser un driver exec sépcifique  
--**name** Pour identifier un conteneur par un nom au lieu d’un ID  
--**dns** Pour définir un DNS personnalisé  
--**net=""** Pour définir le mode réseau entre “Bridge”, “none”, “container:” et “host”  
--**add-host** Modifie le contenu du fichier “hosts” en y ajoutant les valeurs spécifiées  
--**link** Permet d’ajouter un lien vers un autre conteneur  
-**c** Permet de créer un partage  
-**v** Permet de lier un un dossier sur le serveur au conteneur  

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
