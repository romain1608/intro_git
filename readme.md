# Test git 


1ers pas en mardown

*Vous pouvez utiliser _ ou * autour d'un mot pour le mettre en italique. Mettez-en deux pour le mettre en gras.*

## insertion d'une image
![la belle image](./img/image.jpg)

<img src="./img/image.jpg" alt="la belle image" 
	width="200" height="300" 
	style="border: 2px solid blue;
	float: right;">

## lien
[la documentation de Framasite](https://docs.framasoft.org/fr/grav/)

## code
``` select * from la_plage ```

```bash
 sudo apt upgrate
```
## tableau
| Aligné à gauche  | Centré          | Aligné à droite |
| :--------------- |:---------------:| -----:|
| gauche  |   ce texte        | droite |
| gauche  | est             |  droite |
| gauche  | centré          |   droite |
 
## liste
 listes avec les caractères * et - pour des listes non ordonnées ou avec des nombres pour des listes ordonnées.
* jambon
* fromage
  * jambon fromage 
1. fraises
2. framboises  
 
## Découverte git

### 1-Création du dossier et du readme.md en local
C:\rc\A5\github\ **repertoire_git**  
  <span style="color: red"> texte de couleur <span/>


### 2-Installation de git
via debian
```bash
sudo apt update 
sudo apt list git*
idgeo@GS4:~$ sudo apt install git-all
``` 
#### création du repository (**.git**) depuis le dossier:\
   idgeo@GS4:/mnt/c/rc/A5/github/repertoire_git$
   initilalisation du dépot local
```bash
 git init 
 ``` 
 (/ dans linux = à la racine, sinon dossier courant)
#### vérification du statut => connaitre les fichiers commités
```
git status
```
------------------------------------------------------
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        img/
        readme.md

nothing added to commit but untracked files present (use "git add" to track)

--------------------------------------------------------------------

#### configuration des utilisateurs
```git config --global user.email "romaincpgeom@gmail.com"```
```git config --global user.name "romain1608"```

#### versement des fichiers / dossiers

```git add *```  ajoute tout   
```git add readme.md```  ajoute fichier  
 
```git commit -m "1er versement"``` 

--------------------------------------------------  
idgeo@GS4:/mnt/c/rc/A5/github/repertoire_git$ git commit -m "1er versement"
[master (root-commit) cced0f2] 1er versement
 2 files changed, 46 insertions(+)
 create mode 100644 img/image.jpg
 create mode 100644 readme.md
 
 ------------------------------------------------------
 
vérification:   idgeo@GS4:/mnt/c/rc/A5/github/repertoire_git$ git status
```git status```
On branch master
nothing to commit, working tree clean 

###### pour modifier le md dans bash
```nano readme.md```

#### voir les logs
```git log``` 
 
-------------------------------------------
idgeo@GS4:/mnt/c/rc/A5/github/repertoire_git$ git log
commit cced0f218b79320fc7b4b3d8da5720f19a781dc8 (HEAD -> master)
Author: romain1608 <romaincpgeom@gmail.com>
Date:   Mon Sep 9 12:06:56 2024 +0200
1er versement

------------------------------------------

