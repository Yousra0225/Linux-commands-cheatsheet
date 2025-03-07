# Linux terminal cheatsheet

## Commandes

### Navigation / Gestion de dossiers

### Manipulation de fichiers

| Commande | Description | Exemple |
|--|--|--|
`cat [OPTION(S)] [FICHIER(S)]` | Montre le contenu d'un ou plusieurs fichiers.  | `cat input.txt - append.txt`<br>Montre le contenu de input.txt, stdin, et append.txt.
`touch `<ins>`FICHIER`</ins> | Créer un fichier ou modifier la date de modification.<br>`-c`: Ne pas créer de fichier. | `touch text.txt` Créé le fichier text.txt, ou s'il n'existe pas, modifie sa date.
`head [OPTION(S)] `<ins>`[FICHIER(S)]`</ins> | Montre le début d'un (ou de) fichier(s).<br>`-q`: Ne pas afficher les en-têtes (plusieurs fichiers)<br>`-c `<ins>`[-]NB_OCTETS`</ins> / `-n `<ins>`[-]NB_LIGNES`</ins><br>Que les premiers octets/lignes. Le `-` montre tout sauf les derniers octets/lignes. | `head README.md test.txt -n 5`<br>Affiche les 5 premières lignes de README.md et test.txt.
`tail [OPTION(S)] `<ins>`[FICHIER(S)]`</ins> | L'inverse de head, part de la fin plutôt que du début. | `head README.md test.txt -n 5`<br>Affiche les 5 dernières lignes de README.md et test.txt.

### Permissions

### Raccourcis

### Divers

## Bash vs zsh

### Installation

## Frameworks

### Installation
