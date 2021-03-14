# Fonctions

## Exercice 1 : fonctions simples

Commandes utiles : `df`, `who`.

Écrire un script `audit.sh` :

* Écrire une fonction `users_connect` qui affichera la liste des utilisateurs actuellement connectés.

* Écrire une fonction `disk_space` qui affichera l’espace disque disponible.

* Le programme principal affichera le menu suivant :

```
- 0 - Fin 
- 1 - Afficher la liste des utilisateurs connectes 
- 2 - Afficher l’espace disque 
Votre choix :
```

Saisir le choix de l’utilisateur et appeler la fonction adéquate.

## Exercice 2 : fonctions simples, statut de retour

Commandes filtres utiles : `awk`, `tr -d` 
Autres commandes utiles : `df`, `find`.

**Écrire un script watch_sf.sh :**

### Programme principal :

- Le programme principal affichera le menu suivant

```
        0 - Fin 
        1 - Supprimer les fichiers de taille 0 sous mon repertoire d’accueil 
        2 - Controler l’espace disque du SF racine 
        Votre choix :
```

- Saisir le choix de l’utilisateur.

- Le choix 0 provoquera la terminaison du script.

- Le choix 1 provoquera l’appel de la fonction **scan**.

- Le choix 2 provoquera l’appel de la fonction **no_space**.

- En fonction de la valeur renvoyée par la fonction, afficher le message adéquat. 

- Écrire la fonction **scan** : recherche, à partir du répertoire d’accueil de l’utilisateur, tous les fichiers ayant une taille à 0 dans le but de les supprimer (avec demande de confirmation pour chaque fichier).

- Écrire la fonction **no_space** : cette fonction teste le taux d’occupation du système de fichiers racine et renvoie vrai si ce taux est supérieur à 80 %, faux dans le cas contraire.

### Exemples d’exécution

```
$ watch_sf.sh 
 
0 - Fin 
1 - Supprimer les fichiers de taille 0 sous mon repertoire d’accueil 
2 - Controler l’espace disque du SF racine 
Votre choix : 1 
rm: détruire fichier régulier vide  
'/home/vagrant/f1'? n 
etc. 
```

```
$ watch_sf.sh 
 
0 - Fin 
1 - Supprimer les fichiers de taille 0 sous mon repertoire d’accueil 
2 - Controler l’espace disque du SF racine 
Votre choix : 2 
Taux d’occupation du SF racine : NORMAL
```

## Exercice 3 : passage de paramètres, retour de valeur

Écrire un script `calcul.sh` qui contiendra :

- Une fonction **isNombre** qui reçoit une valeur en argument et qui retourne vrai si la valeur est un nombre entier, faux dans le cas contraire. Si vous définissez des variables, elles devront être locales.

- Une fonction **somme** qui reçoit un nombre quelconque de paramètres (en principe, des nombres). La fonction doit vérifier, à l’aide de la fonction **isNombre**, que les arguments reçus sont des nombres et affiche la somme des arguments. Si l’un des arguments est incorrect, il sera ignoré. Si vous définissez des variables, elles devront être locales.

- Une fonction produit qui reçoit un nombre quelconque de paramètres (des nombres). La fonction doit vérifier, à l’aide de la fonction **isNombre**, que les arguments reçus sont des nombres et affiche le produit des arguments. Si l’un des arguments est incorrect, il sera ignoré. Si vous définissez des variables, elles devront être locales.

- Le programme principal :

    - Le script `calcul.sh` recevra en arguments l’opération à réaliser, ainsi qu’une suite de nombres.

        ```
        $ calcul.sh produit 3 5 10  
        150 
        $ calcul.sh somme 3 5 10  
        25
        ```

    - Appeler la fonction correspondant à l’opération demandée et lui transmettre les valeurs reçues par le script. Afficher à l’écran le résultat retourné par la fonction.

## Exercice 4 : fichiers

Commande utile : `printf`

Soit le fichier de données suivant :

```
$ cat eleves.txt  
Nom|Classe|Moyenne 
Lazare|6eme|12 
Cage|6eme|14 
Clareda|6eme|16 
Jougue|6eme|18 
Pingouin|6eme|8 
Dupont|5eme|10 
Durant|5eme|11 
Petit|5eme|7 
Voisin|5eme|14
```

Écrire un script `stats.sh` qui affiche à l’écran, de manière formatée, les trois colonnes du fichier, comme ceci :

```
$ stats.sh  
Nom            Classe       Moyenne 
Lazare         6eme              12 
Cage           6eme              14 
Clareda        6eme              16 
Jougue         6eme              18 
Pingouin       6eme               8 
Dupont         5eme              10 
Durant         5eme              11 
Petit          5eme               7 
Voisin         5eme              14
```

