# DinoDiner

Bienvenue sur le dépôt de l'application DinoDiner.Cette application est une API REST pour gérer les menus du DinoDiner.

La version v1.1 est là ! Téléchargez vite le .jar dans les releases du dépôt.

## Utilisation

Pour lancer l'application, positionnez-vous dans le répertoire dans lequel vous avez placé le fichier .jar et, dans un termnial lancer le script suivant :

```shell
$ java -jar cantina-project-0.0.1-SNAPSHOT.jar
```
Une fois l'appli lancé, dans un autre terminal lancer :

```shell
$ curl -XGET localhost:8080/menus

# Créer un nouveau menu "Menu de Noel" avec un plat "Céréales sur lait"
$ curl -H "Content-Type: application/json"  -d '{"name": "Menu de Noel", "dishes": [{"name": "Céréales sur lait"}]}' http://localhost:8080/menus
```
ou alors taper : "localhost:8080/menus" dans votre naviagteur.

Pour ajouter un menu, vous pour utiliser le terminal de cette façon :

```shell
$ curl -H "Content-Type: application/json"  -d '{"name": "Menu du diplodocus", "dishes": [{"name": "Feuilles d'eucalyptus"}]}' http://localhost:8080/menus
```
Observez votre page web "localhost:8080/menus" !

Note de l'équipe de développement :
Que font des dinosaures qui n'arrivent pas à se décider ?
.
.
.
.
.
Un tirageausaure !
