# Bases
## Exercice 1 : Génération de noms de fichiers

Soit la liste de fichiers suivante :

```
$ ls 
bd.class.php    header.inc.php  install.txt     readme.txt 
essai           index.php       mail.class.php
```

1. Afficher les noms de fichiers se terminant par .php.

2. Afficher les noms de fichiers ayant la lettre e en deuxième position.

3. Afficher les noms de fichiers dont la première lettre est comprise entre a et e.

4. Afficher les noms de fichiers qui ne commencent pas par une voyelle.

### Expressions complexes 

5. Afficher les noms de fichiers qui ne se terminent pas par .php.

6. Afficher les noms de fichiers qui ne se terminent ni par .txt ni par .php.

## Exercice 2 : Séparateur de commandes

Comment écrire les deux commandes suivantes sur la même ligne ?

```
$ cd /tmp 
$ ls -l
```

# Redirections

## Exercice 1

Lister tous les processus du système et rediriger le résultat dans un fichier.

## Exercice 2

Soit la commande who -A, qui génère un message d’erreur :

```
$ who -A 
who : option invalide -- ’A’
```

1. Relancer cette commande et rediriger les erreurs dans un fichier.

2. Relancer cette commande et faire disparaître les erreurs, sans les rediriger dans un fichier disque.

## Exercice 3

### Exécuter les commandes suivantes :

```
$ touch fic_existe 
$ chmod 600 fic_existe  fic_existepas 
chmod: impossible d’accéder à "fic_existepas": Aucun fichier ou 
dossier de ce type
```

1. Rediriger les résultats de la commande chmod dans un fichier, les erreurs dans un autre.

2. Rediriger les résultats et les erreurs de la commande dans un même fichier. 

## Exercice 4

Que fait la commande suivante ?

`$ ls > resu -l`

## Exercice 5

Lancer les commandes date, who et ls et récupérer le résultat de ces trois commandes dans un fichier (une seule ligne de commande).

## Exercice 6

Lancer les commandes `date` et `who -A` et stocker l’affichage de ces deux commandes dans un fichier resu (une seule ligne de commande). 

**Rappel :** la commande `who -A` génère un message d’erreur.

# Tubes

## Exercice 1

Afficher la liste des processus, en paginant l’affichage.


## Exercice 2

En combinant les commandes `ps` et `grep`, afficher la liste des processus sshd qui tournent sur le système.

## Exercice 3

En combinant les commandes tail et head, afficher la sixième ligne du fichier `/etc/passwd`.

## Exercice 4

**Créer les fichiers suivants :**

`$ touch f2 f1 fic1.txt FIC.c Fic.doc fIc.PDF fic` 

Compter le nombre de fichiers dont le nom contient le mot `fic`. La recherche devra être insensible à la casse.
