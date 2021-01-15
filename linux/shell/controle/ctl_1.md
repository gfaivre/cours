1. Citer 3 interpréteurs
2. A quoi sert un interpréteur ? 
3. Qu'affiche la commande `ls /etc/se[r-z]??ces` ? Et Pourquoi ?
4. Expliquer ce que font repsectivement les options `-a` et `-l` de la commande `ls`
5. Comment obtenir des informations sur l'utilisation d'une commande ?
6. À quoi sert la commande `df` ?
7. Quel fichier permet de monter automatiquement les différents systèmes de fichier (partitions) du système ?
8. Qu'est ce que le **prompt** ?
9. Comment afficher l'unique ligne contenant le mot `root` du fichier `/etc/passwd` ?
10. Qu'est-ce qu'un noeud d'indexe (inode) ? 
11. A quoi sert la table des inodes ?
12.  Que se passe t'il lorsque le système n'a plus d'inode disponible ?
13.  Qu'elle est la différence entre un lien physique et un lien symbolique ? 
14.  Donner un exemple de fichier dit «spécial»
15.  Donner un exemple de fichier dit «de communication»

16. Comment afficher la liste de toutes les variables d'environnement d'un shell ?
- [ ] `set`
- [ ] `set -o`
- [ ] `env`
- [ ] Aucune de ces réponses

17. Quelle sont les affirmations vraies ci-dessous ?
- [ ] La commande alias permet de créer un «synonyme» pour une commande
- [ ] La commande `unalias` permet de supprimer un alias
- [ ] La commande `alias -l` permet de lister les alias définis
- [ ] Un alias est automatiquement exporté dans les shells enfants

18. Que se passe t-il lorsque cette commande est exécutée: `ls > resu`
- [ ] Le shell créé ou écrase le fichier **resu** puis la commande **ls** écrit dans le fichier **resu**.
- [ ] La commande **ls** crée ou écrase le fichier **resu**, puis écrit dans le fichier **resu**
- [ ] Aucune de ces réponses

19. Quelles sont les commandes correctes pour rediriger tous les affichages dans le même fichier?

[ ] `find / -name test.php 1> resu 2> resu`
[ ] `find / -name test.php 1> resu 2>> resu`
[ ] `find / -name test.php 1> resu 2&1`
[ ] `find / -name test.php 2> resu 1&2`
[ ] `find / -name test.php 1> resu 1>&2 2>resu`
[ ] Aucune de ces propositions

20. Comment rediriger la sortie standard de toutes ces commandes dans le même fichier ? 

[ ] `cd /tmp ; pwd ; ls > listefic`
[ ] `{ cd /tmp ; pwd ; ls } > listefic`
[ ] `[ cd /tmp ; pwd ; ls ] > listefic`
[ ] `( cd /tmp ; pwd ; ls ) > listefic`
[ ] Aucune de ces propositions
