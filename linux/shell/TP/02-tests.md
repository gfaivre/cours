# Tests

Ces exercices ne nécessitent pas l’emploi de la structure de contrôle if. Seules les commandes [ ], [[ ]], expr, (( )) et $(( )) sont utilisées. Afficher le statut de retour des commandes pour savoir si la commande retourne vrai (0) ou faux (>0).

## Exercice 1 : Tests sur des fichiers

1. Tester si le fichier (ou répertoire) /etc existe.

2. Tester si le fichier /etc/hosts est accessible en lecture.

3. Tester si le fichier /etc/hosts est exécutable.

4. Tester si le fichier /usr est un répertoire et s’il est traversable.

5. Tester si le fichier /dev/null est un fichier spécial périphérique.

b. Exercice 2 : tests de chaînes de caractères

**Définir les variables suivantes :**

```
$ s1=oui 
$ s2=non 
$ vide="" 
$ fic1=rapport.pdf
```

1. Tester si $s1 est égale à $s2.

2. Tester si $s1 est différente de $s2.

3. Tester si $vide est vide.

4. Tester si $vide n’est pas vide.

5. Tester si $fic1 se termine par .doc (bash/ksh uniquement).

6. Tester si $fic2 se termine par .doc ou par .pdf.

## Exercice 3 : Tests numériques

Définir les variables nb1 et nb2 avec les valeurs suivantes :

```
$ nb1=2 
$ nb2=100
```

Tester si $nb1 est strictement supérieure à $nb2 à l’aide des commandes [ ], [[ ]] et (( )).

## Exercice 4 : Arithmétique

En ligne de commande, initialiser deux variables numériques nb1 et nb2 :

```
$ nb1=3  
$ nb2=5
```

1. Initialiser une variable res avec la somme de nb1 et nb2. Afficher res. 

2. Sans initialiser de variable res, afficher à l’écran la somme des deux nombres. 

3. Initialiser une variable res avec le résultat de la multiplication de nb1 et nb2. Afficher res.

## Exercice 5 : opérateurs logiques des commandes [ ] et [[ ]] et opérateurs logiques du shell

Lancer les commandes suivantes :

```
$ > fic 
$ chmod 444 fic 
$ ls -l fic 
-r--r--r-- 1 vagrant vagrant 0  2 avril 17:23 fic
```

1. Si le fichier $ n’est pas exécutable, afficher "Droit x non positionné".

2. Si le fichier $fic n’est ni exécutable ni accessible en écriture, afficher "Droits wx non positionnés".
