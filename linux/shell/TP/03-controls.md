# Structures de contrôle if, case, boucle for

## Exercice 1 : les commandes [ ] et [[ ]], la structure de contrôle if

Commandes filtres utiles : `awk`

Écrire un script `compare.sh` :

* Nombre d’arguments reçus : deux noms de fichiers ordinaires.

* Vérifier que le nombre d’arguments est égal à 2 et que les fichiers sont de type ordinaire.

* Si les arguments sont corrects, le script doit dire si les deux fichiers ont la même taille ; si ce n’est pas le cas, il doit dire quel est le fichier le plus grand.

### Exemple:

```
$ compare.sh  /etc/hosts  
Usage : ./compare2.sh fichier1 fichier2 
 
$ compare.sh  /etc/hosts /etc/passwd 
Le fichier /etc/passwd a la plus grande taille : 1910 octets 
Bye ...
```

## Exercice 2 : structures de contrôle case, boucle for

Écrire un script `typefic.sh` qui prend des noms de fichiers en arguments. Si le fichier se termine par **.doc** ou **.pdf**, afficher un message spécifique. Sinon afficher "Ni DOC, ni PDF".

### Exemple:

```
$ typefic.sh f1.doc f2.pdf f3.txt  
f1.doc : Fichier DOC 
f2.pdf : Fichier PDF 
f3.txt : Ni DOC, ni PDF
```


