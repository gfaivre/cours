# Boucles

## Exercice 1 : boucle for, commande tr

Commandes filtres utiles : `tr`. 
Autres commandes utiles : `mv`

### Écrire un script maj_min.sh :

* Argument facultatif : un nom de répertoire. La valeur par défaut de l’argument sera le répertoire courant.

* Vérifier que l’éventuel argument est un répertoire.

* Ce script renommera les noms de fichiers de ce répertoire : les noms de fichiers majuscules seront convertis en minuscules.

## Exercice 2 : boucle for, arithmétique

Commandes filtres utiles : `grep`, `wc`. 
Autres commandes utiles : `ps`.

Écrire un script `proc_users.sh` :

* Arguments : un ou plusieurs noms d’utilisateurs.
* Tester le nombre d’arguments reçus : il doit y avoir au moins un argument.
* Pour chaque utilisateur reçu en argument, afficher à l’écran le nombre de processus appartenant à ce dernier. Si l’utilisateur n’est pas défini sur le système, il sera ignoré.

### Exemples

```
$ proc_users.sh  
Usage : ./proc_users.sh user1 user2 ... usern 
```

``` 
$ proc_users.sh christie olivier daniel 
L’utilisateur vagrant fait tourner 8 processus 
L’utilisateur ssd n’a pas de processus 
rix n’est pas un utilisateur valide
```

## Exercice 3 : boucles for, while

Commandes filtre utile : `grep`
Autres commandes utiles : `file`, `find`.

### Écrire un script `consulte.sh` :

* Argument facultatif : un nom de répertoire. Vérifier que l’argument reçu est un répertoire.

* Si le script ne reçoit pas de nom de répertoire, traiter le répertoire courant.

* Rechercher tous les fichiers ordinaires qui sont sous ce répertoire (à tous les niveaux).

* Pour chaque fichier de contenu texte accessible en lecture, demander à l’utilisateur s’il veut consulter le fichier. Un fichier non texte sera ignoré.

* L’utilisateur pourra saisir ’o’, ’O’, ’oui’, ’OUI’ pour consulter le fichier, ’n’, ’N’, ’non’, ’NON’ pour ne pas le consulter, ou ’q’ pour quitter le script. Toute autre réponse engendrera une nouvelle demande de saisie.

    * Si l’utilisateur souhaite consulter le fichier : afficher le contenu paginé du fichier à l’écran.

    * Si l’utilisateur ne souhaite pas consulter le fichier : passer au fichier suivant. 

