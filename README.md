# Linux terminal cheatsheet

## Commandes

### Navigation / Gestion de dossiers
------------------------------------
-----------------------------------
|Commande|Description|Exemple|
|--------|-----------|-------|
|`pwd`|Affiche le chemin du répertoire courant|`pwd` : `/home/user/cda`|
|`ls`|Liste les fichiers et dossiers|`ls` : `dossier1 fichier1 ...`|
|`ls -l`|Affiche les fichiers avec des détails supplémentaires|`ls -l` : `taille permission ...`|
|`ls -a`|Affiche les fichiers et dossiers, y compris les fichiers cachés|`ls -a` : `.fichier`|
|`ls -R`|Affiche les fichiers et sous-dossiers récursivement|`ls -R` : `dossier1 fichier1 -> dossier1 -> dossier2 fichier2 ...`|
|`rm fichier`| Supprime un fichier | `rm fichier.txt` |
|`cp -r dossier destination`| Copie un dossier | `cp -r projet /home/user/backup/` | 



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
#### Raccourcis pour Bash

| Navigation | Description                           |
| ---------- | ------------------------------------- |
| CTRL + A   | Aller au début de la ligne            |
| CTRL + E   | Aller à la fin de la ligne            |
| CTRL + B   | Se déplacer d'un caractère en arrière |
| CTRL + F   | Se déplacer d'un caractère en avant   |
| ALT + B    | Se déplacer d'un mot en arrière       |
| ALT + F    | Se déplacer d'un mot en avant         |


| Édition  | Description                                                                 |
| -------- | --------------------------------------------------------------------------- |
| CTRL + U | Couper ou effacer depuis la position du curseur, jusqu'au début de la ligne |
| CTRL + L | Couper ou effacer depuis la position du curseur, jusqu'à la fin de la ligne |
| CTRL + W | Couper ou effacer le mot avant le curseur                                   |
| CTRL + Y | Coller le dernier contenu coupé                                             |
| CTRL + L | Vider le terminal                                                           |


| Historique | Description                                     |
| ---------- | ----------------------------------------------- |
| CTRL + R   | Rechercher dans l'historique                    |
| CTRL + G   | Sortir de la recherche dans l'historique        |
| CTRL + P   | Donner la précédente commande dans l'historique |
| CTRL + N   | Aller à la prochaine commande dans l'historique |
| CTRL + C   | Arrêter la commande en cours                    |

#### Raccourcis zsh
**Note :** les raccourcis zsh sont majoritairement similaire à ceux de Bash.
| Raccourcis | Description                                                  |
| ---------- | ------------------------------------------------------------ |
| Alt + W    | Effacer de la position du curseur jusqu'au début de la ligne |
| CTRL + X + CTRL + E | Démarrer l'éditeur texte par défaut                 |
| CTRL + X + CTRL + X | Sélectionner la ligne du début jusqu'à la position du curseur |



#### Raccourcis Nano
| Raccourcis          | Description                                                             |
| ------------------- | ----------------------------------------------------------------------- |
| CTRL + O            | Sauvegarder le fichier                                                  |
| CTRL + X            | Quitter Nano (avec proposition de sauvegarde si fichier non sauvegardé) |
| CTRL + Y            | Remonter d'une page                                                     |
| CTRL + V            | Descendre d'une page                                                    |
| Alt + \             | Aller à une ligne spécifique                                            |
| Alt + ,             | Aller au début de la ligne                                              |
| Alt + .             | Aller à la fin de la ligne                                              |
| CTRL + K            | Couper/Effacer à partir du curseur jusqu'à la fin de la ligne           |
| CTRL + U            | Annuler couper/Restaurer le texte coupé                                 |
| CTRL + 6            | Créer un bloc de texte pour qu'il soit copié ou coupé                   |
| CTRL + 6 & CTRL + K | Couper/Effacer le bloc de texte                                         |
| Alt + 6             | Copier le bloc de texte                                                 |
| CTRL + W            | Rechercher du contenu dans le texte                                 |
| Alt + W             | Rechercher et remplacer du contenu                                      |
| Alt + R             | Répéter la précédente recherche                                         |

#### Raccourcis Vim
**Mode normal** 
| Raccourcis | Desciption                                                                 |
| ---------- | -------------------------------------------------------------------------- |
| i          | Entrer en mode insertion à la position actuelle du curseur                 |
| x          | Effacer le caractère sous le curseur                                       |
| dd         | Effacer la ligne                                                           |
| yy         | Copier la ligne                                                            |
| p          | Coller le contenu qui a été copié ou coupé en dessous de la ligne actuelle |
| u          | Annuler la dernière action                                                 |
| CTRL + R   | Reproduire à nouveau la dernière action                                    |

**Mode commande**
| Raccourcis        | Description                                               |
| ----------------- | --------------------------------------------------------- |
| :w                | Sauvegarder le fichier                                    |
| :q                | Quitter Vim                                               |
| :q!               | Quitter Vim sans sauvegarder                              |
| :wq               | Sauvegarder et quitter Vim                                |
| :s/avant/après/g  | Changer le contenu d'"avant" par celui voulu dans "après" |
| :set nu ou number | Afficher le nombre de lignes                              |

**Mode visuel**
| Raccourcis | Description                                      |
| ---------- | ------------------------------------------------ |
| v          | Entrer en mode visuel pour sélectionner du texte |
| y          | Copier le texte sélectionné                      |
| d          | Effacer la zone de texte sélectionné             |
| p          | Coller le texte copié ou coupé                   |


### Divers

## Bash vs zsh

### Installation

## Frameworks

### Installation
