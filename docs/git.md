# 📘 Fiche Technique Complète : Git, Python et MkDocs

> **Référentiel :** Gestion de projet, versioning, déploiement de documentation.
> **Usage :** Création de projet Python, suivi Git, déploiement MkDocs sur GitHub Pages.

---

## Identité du Projet
* **Nom Officiel :** cpgeom_docs
* **Auteur :** Abdoulhakim Elmi
* **Technologies :** Python 3, Git, MkDocs, GitHub Pages
* **Objectif :** Créer un projet documenté avec versioning Git et déploiement automatique de documentation.

---

## 1️⃣ Préparation de l’environnement

### 1.1 Accéder au projet

```
cd /mnt/h/cpgeom_docs
ls -la
```


1.2 Installer Python et outils

```
sudo apt update
sudo apt upgrade -y
sudo apt install python3-venv python3-pip
python3 --version
pip3 --version
```

python3-venv : pour créer un environnement virtuel.

pip3 : pour installer les packages Python.

2️⃣ Créer un environnement virtuel
```
python3 -m venv .venv
source .venv/bin/activate


.venv : dossier contenant l’environnement virtuel.
```
source .venv/bin/activate : active l’environnement pour installer les packages localement.


3️⃣ Installer MkDocs et initialiser le projet
```
pip install mkdocs
touch mkdocs.yml
mkdocs serve
```


mkdocs serve : lance un serveur local pour prévisualiser le site.

4️⃣ Initialiser Git
```
git init
git status
```

Crée un dépôt Git local et vérifie l’état des fichiers.

4.1 Configurer l’identité Git
```
git config --global user.name "Abdoulhakim Elmi"
git config --global user.email "abdoulhakim.elmi@gmail.com"
git config --global --list
```


Configure ton identité pour signer les commits.

5️⃣ Premier commit
```
git add .
git commit -m "premier commit"
```


git add . : ajoute tous les fichiers au suivi.

git commit -m : crée un commit avec un message.

6️⃣ Connecter GitHub et pousser le projet
```
git remote add origin https://github.com/abdoulhakimelmi-lang/cpgeom.git
git branch -M main
git push -u origin main
```


origin : nom du dépôt distant.

branch -M main : renomme la branche principale en main.

-u origin main : configure la branche main pour le push futur.

7️⃣ Déploiement MkDocs sur GitHub Pages
```
mkdocs gh-deploy
```

Publie automatiquement le site sur GitHub Pages.

Le site sera accessible via l’URL du dépôt GitHub.

8️⃣ Sauvegarde de l’historique des commandes
```
history > mon_history.txt
```


Permet de sauvegarder toutes les commandes utilisées dans un fichier texte pour référence future.