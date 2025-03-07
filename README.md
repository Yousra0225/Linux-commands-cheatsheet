# Linux terminal cheatsheet

## Commandes

### Navigation / Gestion de dossiers

### Manipulation de fichiers

| Commande | Description | Exemple |
|--|--|--|
`cat [OPTION(S)] [FICHIER(S)]` | Montre le contenu d'un ou plusieurs fichiers.  | `cat input.txt - append.txt`<br>Montre le contenu de input.txt, stdin, et append.txt.
`touch `<ins>`FICHIER`</ins> | Créer un fichier ou modifier la date de modification.<br>`-c`: Ne pas créer de fichier. | `touch text.txt`<br>Créé le fichier text.txt, ou s'il n'existe pas, modifie sa date.
`head [OPTION(S)] `<ins>`[FICHIER(S)]`</ins> | Montre le début d'un (ou de) fichier(s).<br>`-q`: Ne pas afficher les en-têtes (plusieurs fichiers)<br>`-c `<ins>`[-]NB_OCTETS`</ins> / `-n `<ins>`[-]NB_LIGNES`</ins><br>Que les premiers octets/lignes. Le `-` montre tout sauf les derniers octets/lignes. | `head README.md test.txt -n 5`<br>Affiche les 5 premières lignes de README.md et test.txt.
`tail [OPTION(S)] `<ins>`[FICHIER(S)]`</ins> | L'inverse de head, part de la fin plutôt que du début. | `head README.md test.txt -n 5`<br>Affiche les 5 dernières lignes de README.md et test.txt.
`tail`, pour suivre des modifications | `-f`: Montre les changements lorsqu'ils arrivent, suit le fichier même à travers les renommages.<br>`--follow=name`: Suit uniquement le fichier du même nom.<br>`--retry`: Réessayer de lire lorsque l'accès est refusé.<br>`-s`: Temps avec retry. | `tail README.md -F`<br>Lit le README dans son entièreté, montre les mises à jour 
<ins>`TEXTE`</ins>` > `<ins>`FICHIER`</ins> | Insère le texte (en dur, d'une commande) au fichier. | `head README.md -n 5 > test.txt`<br>Copie les 5 premières lignes de README.md dans le fichier test.txt.

### Permissions

### Raccourcis

### Divers

## Bash vs zsh

### Installation

## Frameworks

### Installation
