# Docker-TP2

## Compléter le Dockerfile afin de builder correctement l’application contenu dans src/

Pour installer uniquement les dépendances nécessaires, utilisez l'option npm --prod ou -p, qui évite d'installer les dépendances de développement.
Une bonne pratique avec Docker consiste à séparer les images de production et de développement afin d'éviter d'installer les dépendances de développement dans l'image de production et ainsi réduire la taille de l'image.

## A l’aide de la commande docker build, créer l’image my_app

Utilisez la commande suivante pour construire votre image à partir du fichier Dockerfile et l'appeler ma_super_app :

``` docker build -f Dockerfile -t ma_super_app . ```


## Compléter le fichier docker-compose.yml afin d’éxécuter ma_super_app avec sa base de données.

Consultez le fichier docker-compose.yml.
Dans le fichier .env, ajoutez les variables d'environnement suivantes :
makefile

```
NODE_ENV=production
MYSQL_DATABASE=tp02
MYSQL_USER=root
MYSQL_PASSWORD=root 
```