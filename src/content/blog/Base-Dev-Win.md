---
title: "[Dev] Le starterPack pour Windows"
description: "StarterPackDev"
pubDate: "Jul 27 2023"
heroImage: "/vscodeanime.jpg"
---

Voici un petit guide rapide pour installer et utiliser votre environnement pour dévlopper.

## Git/GitHub :

En premier lieu, il faudra installer un nouveau terminal, à savoir GitBash. GitBash ressemble à ceci :
![Ex1](https://gitforwindows.org/img/gw1.png)

Faut pas avoir peur, car c'est juste un terminal Unix, mais pour Windows. Ça mange pas de pain et c'est plutôt cool. Pendant l'installation, il faudra cocher les éléments ci-dessous :

- Windows Explorer Integration
- Git Bash Here
- Git LFS (Large File Support)
- Associate .git\* configuration files with the default text editor
- Associate .sh files to be run with Bash
- Add a Git Bash Profile to Windows Terminal
- Scalar (Git add-on to manage large-scale repositories) ..

Ensuite, tu choisis : _"Use Visual Studio Code as Git's default editor"_. Coche ensuite _"Override the default branch name for new repositories"_, et dans le champ de texte, garde l'option proposée "main", puis coche l'option recommandée _"Git from the command line and also from 3rd-party software"_.

Et continue dans le cochage, car tu vas devoir cocher :
_"Use Bundled OpenSSH"_
_"Use The OpenSSL library"_
_"Checkout as-is, commit Unix-style line endings"_
_"Use MinTTY (the default terminal of MSYS2)"_

On garde l'option par défaut _"Default (fast-forward or merge)"_.

On sélectionne _"none"_, il n'est pas utile d'installer le git credential manager car on va mettre en place l'authentification en SSH par la suite.

Et on recoche deux nouvelles options :
_"Enable file system caching"_
_"Enable Symbolic links"_

Allez courage, on a bientôt fini avec le cochage, donc tu vas cocher :
_"Enable experimental support for pseudo consoles"._
Tu peux aussi, si tu le souhaites, cocher la seconde option _"Enable experimental built-in file system monitor"_...

Voilà on a terminé pour l'installation, mais on a encore quelque éléments à rajouter :

- Renseigne ton nom d'utilisateur : `git config --global user.name "FIRST_NAME LAST_NAME"`
- Renseigne ton email : `git config --global user.email "MY_NAME@example.com"`

### Maintenant le SSH :

Alors, pour continuer, on va devoir récupérer Chocolatey.

( https://chocolatey.org/install#individual ) _Si tu suis les indications , tout ira bien_.

Allez, maintenant on va installer GitHub CLI : `choco install gh`
Ensuite, tu vas taper `gh`. Le CLI est installé.

Pour la création du SSH, GitHub a fait un excellent tutoriel que tu vas suivre à la lettre:

https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

Voilà, la partie Git est installée et prête à l'utilisation. Maintenant, essaie de créer un dépôt, un Readme.md, et suis les principes de Git _(Add, commit, push)_.

## Installation de Visual Studio Code ou VsCodium :

Maintenant, je te propose d'installer Visual Studio Code. Il y a d'autres IDE (Integrated Development Environments) comme :

- Visual Studio Code
- Sublime Text
- Vim

Pour télécharger le Visual Studio Code :
[Visual Studio Code](https://code.visualstudio.com/ "Lien vers Visual Studio Code ").

Pour télécharger VSCodium : [VsCodium](https://vscodium.com/ "Lien vers VSCodium ").

![Ex2](https://storage.googleapis.com/quest_editor_uploads/vpfTdRmeHQosd5vbrQffVu9vmRoOrdaj.png) _Interface de Visual Studio Code_

### Formater le code à chaque sauvegarde :

Tu sais qu'il est possible de configurer ton éditeur de code pour que le code se formate automatiquement lorsque tu sauvegardes. Clique sur _"Settings"_ en bas du menu et sélectionne l'option _"Settings"_.

Cherche dans la barre de recherche _"format"_ et active l'option _"format on save"_. Ferme à présent l'onglet _"Settings"_. Tu peux tester la fonctionnalité en créant une nouvelle balise dans ton document et en sauvegardant.

![Ex3](https://storage.googleapis.com/quest_editor_uploads/FwI80nT2ZP5HEK4Ib8REZItrIyDlZV38.gif)

### Liste d'extension :

- Live Server
- Live Share
- Live Preview
- Better Comments
- CodeSnap
- markdownlint
- Css Snippets
- DotENV
- EsLint
- JavaScript (ES6) code snippets
- Nord Dark Pro

Et voilà, tu as ta petite base pour pouvoir dévlopper. A toi de découvrir ce monde merveilleux et paramétrer à ta guise .
