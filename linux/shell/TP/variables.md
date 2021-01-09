# 1 - Variables et caractères spéciaux

## Exercice 1

1. Définir une variable contenant votre prénom et afficher la.
2. Définir une variable contenant votre prénom suivi de votre nom. Afficher cette variable.
3. Supprimer ces deux variables de manière à ce qu'elles apparaissent comme indéfinies.

## Exercice 2

Définir une variable contenant votre nom et une autre contenant votre prénom. Avec un seul appel à la commande **echo**, afficher ces deux variables, séparées par un espace (votreprenom votrenom).
    
## Exercice 3

1. En une seule commande, afficher la date courante avec le format suivant:

`Nous sommes le sam. févr. 22 14:32:22 CET 2014`

2. Même chose que ci-dessus, mais formater la date comme suit:

`Nous sommes le 22/02/2014`

# 2 Affichages et lectures clavier

## Exercice 1 : Variables

Écrire un script `premier.sh` et réaliser les opérations suivantes :

    Initialiser une variable prenom.

    Initialiser une variable maDate qui contiendra la date courante.

    Afficher ces deux variables.

**Exécuter ce script.**

## Exercice 2 : Paramètres

Écrire un shell script `wcount.sh` qui produit le résultat suivant :

```
$ bash wcount.sh ours oiseau 
Le nom du script est : wcount.sh 
Le 1er argument est : ours 
Le 2eme argument est : oiseau 
Tous les arguments : ours oiseau 
Nombre total d’arguments : 2 
Le 1er argument contient : 4 caracteres 
Le 2eme argument contient : 6 caracteres
```

# Exercice 3 : Lecture clavier

Écrire un script hello.sh qui :

1. Demande à l’utilisateur la saisie de son prénom et le stocke dans une variable. 

2. Demande à l’utilisateur la saisie de son nom et le stocke dans une autre variable.

3. Affiche un message de bienvenue à l’utilisateur.

4. Affiche le PID du shell qui exécute le script.

```
$ hello.sh  
Entrez votre prenom : Christine 
Entrez votre nom : Deffaix Remy 
Bonjour Christine Deffaix Remy, bienvenue ! 
Le PID du shell est 2569
```
