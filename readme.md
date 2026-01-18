# Template – Dépôt de documentation (BTS SIO)

## 1. Objectif du dépôt

Ce dépôt a pour objectif de fournir un modèle simple et réutilisable permettant aux étudiants de **BTS SIO** de stocker, d’organiser et de collaborer sur leur documentation technique de l’atelier de professionnalisation en utilisant **Git** et un dépôt distant comme **GitHub**.

L’idée est de :

- Centraliser la documentation
- Travailler à plusieurs sans écraser le travail des autres
- Garder un historique des modifications
- Appliquer de bonnes pratiques professionnelles

---

## 2. Pourquoi Git existe ?

Avant Git, la gestion de versions était plus limitée et souvent centralisée. Dans les années 2000, le noyau **Linux** était développé à très grande échelle par des milliers de contributeurs.

### ⛓️ BitKeeper

Pour gérer ce volume de contributions, les développeurs du noyau Linux utilisaient un outil propriétaire appelé **BitKeeper**. Ce dernier était performant, mais :
- Il n’était **pas libre**
- Sa licence a posé des problèmes à la communauté open source
- Son usage gratuit a été retiré pour le projet Linux

### ⛓️‍💥 Naissance de Git

En 2005, **Linus Torvalds** décide alors de créer un nouvel outil répondant à des besoins précis :
- Libre et open source
- Décentralisé
- Fiable et sécurisé

Aujourd’hui, Git est devenu le standard mondial de la gestion de versions, utilisé aussi bien en développement logiciel qu’en documentation.

---

## 3. Comment fonctionne Git ?

Git repose sur un fonctionnement **local et distribué**.

### Les trois zones

1. **Working Directory**  
   🔸 Ce sont les fichiers et les dossiers présents sur l’ordinateur.

2. **Staging Area (Index)**  
   🔸 Zone intermédiaire où l’on prépare les modifications.

3. **Repository (local)**  
   🔸 Historique des versions validées (commits).

### Le principe du commit

Un **commit** représente un instantané du projet à un moment donné. Chaque commit :
- Possède un identifiant unique (hash)
- Contient un message descriptif
- Peut être retrouvé ou annulé

Git ne sauvegarde pas simplement des fichiers, mais **l’historique complet du projet**.

> Git ne sauvegarde pas tout le fichier modifié, seulement ce qui a été modifié.

---

## 4. Organisation du dépôt

```

📦 template-ap
┣ 📂 01-mission
┣ 📂 02-mission
┣ 📂 03-mission
┗ 📜 README.md

```

### Bonnes pratiques

- Un dossier par contexte
- Des noms clairs et explicites
- Documentation en **Markdown (.md)**

---

## 5. Utiliser ce dépôt comme template

Ce dépôt est conçu pour être **réutilisé**.

### Cloner depuis l’interface GitHub

1. Cliquer sur **Use this template**
2. Créer ton propre dépôt
3. Modifier le README et les dossiers selon les besoins

> 💡 Dans votre README, vous pouvez expliquer le contexte de l’atelier de professionnalisation ainsi que l’organisation de votre dépôt.

### Cloner depuis le terminal

1. Dans un répertoire contenant vos projets, créer un dossier avec le nom de votre dépôt.
2. Aller dans le dossier et cloner le dépôt template :
```
cd nom-de-votre-repertoire
git clone [https://github.com/AP-BTS-SIO-Louis/template-ap.git](https://github.com/AP-BTS-SIO-Louis/template-ap.git) .
```
3. Supprimer le dossier `.git` :
```
rm -rf .git
```
4. Initialiser Git :
```
git init
```

---

## 6. Utilisation de Git

### Commandes essentielles

```
git status   # Voir l’état du dépôt
git add .    # Ajouter les fichiers à l’index
git commit -m "Message clair"
git pull     # Récupérer les changements distants
git push     # Envoyer ses modifications
```

### Bonnes pratiques

- Toujours faire un `git pull` avant de travailler
- Utiliser des messages de commit clairs
- Ne pas modifier les fichiers des autres sans concertation

---

## 7. Auteur

- **Louis MEDO**
- Étudiant en BTS SIO
- [LinkedIn](https://www.linkedin.com/in/louismedo/) | [Portfolio](https://louis.loutik.fr)
