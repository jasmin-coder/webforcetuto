# webforcetuto
## Tutoriels webforce


#### enter to https://github.com/wingstechno/webforcetuto.git and fork the project


#### cloner le projet chez moi en local
```git  clone FORKED-URL-ADDRESS```


#### vérifier l'url remote en origin et upstream
```git  remote -v```


#### créer un nouveau fichier texte en mon nom depuis mon éditeur texte et je le remplit par du texte (ex : abdelali.txt)


#### vérifier le status de mon repo local (on va voir que le nouveau fichier créé n'est pas encore ajouté au versionning)
```git  status```


#### ajouter le fichier au versionning
```git  add MONNOM.txt```
#### ou bien si on veut ajouter plusieurs fichiers
```git  add .```


#### fichier ajouté au versionning mais pas encore commité au repo local
```git  commit -am "Ajout fichier MONNOM.txt"```


#### on lance cette commande pour savoir à quelle branche on est mnt
```git  branch```


#### le fichier est commité localement mais pas encore envoyé à github...
#### envoyer le fichier au repo distant sur github (dossier upstream)
#### upstream c'est le nom du dossier au repo distant - main c'est le nom de la branche
```git  push upstream main```
##### ça y'est!! on peut voir le fichier dans l'url de github


#### on va créer maintenant une nouvelle branche
```git  branch develop```
##### nouvelle branche créée à partir de la branche courante main
##### dans la nouvelle branche on trouve le contenu et l'historique git de la branche de départ


#### on se déplace à la nouvelle branche maintenant
```git  checkout develop```


#### on fait des changement sur le fichier en notre nom (on rajoute une ou plusieurs lignes)


#### puis on commit les changements faits
```git  commit -am "nouvelle changements branche develop"```
##### chengements envoyés au repo local


#### avant d'envoyer les changements au repo distant, on doit créer ce nouveau dossier, on l'appelle "upstream" et on met dans sa valeur l'url repo github: https://github.com/wingstechno/webforcetuto.git
```git  remote -v```
```git  remote add upstream https://github.com/wingstechno/webforcetuto.git```


#### maintenant on peut envoyer les changements au repo distant dans le dossier upstream
```git  push upstream develop```