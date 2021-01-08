# webforcetuto
## Tutoriels webforce

<p>&nbsp;</p>

#### enter to https://github.com/wingstechno/webforcetuto.git and fork the project

<p>&nbsp;</p>

#### cloner le projet chez moi en local puis entrer au dossier
```git  clone FORKED-URL-ADDRESS```

<p>&nbsp;</p>

#### définir l'url upstream
```git  remote -v```
```git  remote add upstream https://github.com/wingstechno/webforcetuto.git```
```git  remote -v```

<p>&nbsp;</p>

#### créer un nouveau fichier texte en mon nom depuis mon éditeur texte et je le remplit par du texte (ex : abdelali.txt)

<p>&nbsp;</p>

#### vérifier le status de mon repo local (on va voir que le nouveau fichier créé n'est pas encore ajouté au versionning)
```git  status```

<p>&nbsp;</p>

#### ajouter le fichier au versionning
```git  add MONNOM.txt```
#### ou bien si on veut ajouter plusieurs fichiers
```git  add .```

<p>&nbsp;</p>

#### fichier ajouté au versionning mais pas encore commité au repo local
```git  commit -am "Ajout fichier MONNOM.txt"```

<p>&nbsp;</p>

#### on lance cette commande pour savoir à quelle branche on est mnt
```git  branch```

<p>&nbsp;</p>

#### le fichier est commité localement mais pas encore envoyé à github...
#### envoyer le fichier à mon repo distant sur github (origin)
```git push origin main```
##### ça y'est!! on peut voir le fichier dans mon repo github (origin) mais pas au repo distant webforcetuto (upstream)

<p>&nbsp;</p>

#### on va créer maintenant une nouvelle branche
```git  branch develop```
##### nouvelle branche créée à partir de la branche courante main
##### dans la nouvelle branche on trouve le contenu et l'historique git de la branche de départ

<p>&nbsp;</p>

#### on se déplace à la nouvelle branche maintenant
```git  checkout develop```

<p>&nbsp;</p>

#### on fait des changement sur le fichier en notre nom (on rajoute une ou plusieurs lignes)

<p>&nbsp;</p>

#### puis on commit les changements faits
```git  commit -am "nouvelle changements branche develop"```
##### chengements envoyés au repo local

<p>&nbsp;</p>

#### avant d'envoyer les changements au repo distant, on doit créer ce nouveau dossier, on l'appelle "upstream" et on met dans sa valeur l'url repo github: https://github.com/wingstechno/webforcetuto.git
```git  remote -v```
```git  remote add upstream https://github.com/wingstechno/webforcetuto.git```

<p>&nbsp;</p>

#### maintenant on peut envoyer les changements au repo distant dans le dossier upstream
```git  push upstream develop```