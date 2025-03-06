# Linux-commands-cheatsheet

### Navigation / Gestion de dossier
-----------------------------------
|Commande|Description|Exemple|
|--------|-----------|-------|
|`pwd`|Affiche le chemin du répertoire courant|`pwd` : `/home/user/cda`|
|`ls`|Liste les fichiers et dossiers|`ls` : `dossier1 fichier1 ...`|
|`ls -l`|Affiche les fichiers avec des détails supplémentaires|`ls -l` : `taille permission ...`|
|`ls -a`|Affiche les fichiers etdossiers, y compris les fichiers cachés|`ls -a` : `.fichier`|
|`ls -R`|Affiche les fichiers et sous-dossiers récursivement|`ls -R` : `dir1 file1 -> dir1 -> dir2 file2 ...`|
|`cd ..`| Revenir au répértoire parent| `cd ..`|
|`cd /`|Va à la racine du système|`cd /`|
|`cd ~`|Va dans le dossier personnel de l'utilisateur |`$HOME`|
|`cd dossier`| Accède à un répertoire spécifique| `cd /chemin/vers/dossier`|
|`mv fichier`|Déplace ou renomme un fichier|`mv fichier.txt /home/user/docs/`|
|`mv -v fichier`|Affiche les fichiers déplacés ou renommés|`mv -v fichier.txt /home/`|
| `mkdir projet`| Crée un dossier| `mkdir projet`|
| `mkdir -p dossier1/dossier2`  | Crée un dossier avec ses sous-dossiers| `mkdir -p projet/docs`|
| `rmdir dossier`| Supprime un dossier vide| `rmdir dossier_vide`|
| `rm -r dossier`| Supprime un dossier et son contenu | `rm -r projet`|
|`rm fichier`| Supprime un fichier | `rm fichier.txt` |
|`rm -f fichier`|Force la suppression d'un fichier sans demander de confirmation|`rm -f fichier.txt`|
|`touch fichier.txt`| Crée un fichier vide | `touch nouveau_fichier.txt`|
|`cp fichier destination`| Copie un fichier| `cp fichier.txt /home/user/docs/`|
|`cp -r dossier destination`| Copie un dossier | `cp -r projet /home/user/backup/` | 
|`find /chemin -name fichier`| Recherche un fichier par nom| `find /home/user/ -name "document.txt"`|
|`locate fichier`| Trouve rapidement un fichier| `locate fichier.txt`|
