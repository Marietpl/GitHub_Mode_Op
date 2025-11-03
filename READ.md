# GitHub_Mode_Op

---

## 🎯 Objectifs

Apprendre à :

- Créer un projet Git

- Travailler en local dans VS Code

- Utiliser GitHub Desktop + Terminal

- Envoyer son travail sur GitHub

- Récupérer (cloner) un projet GitHub en local

- Faire des branches

---

## 1. Comprendre les outils
| Outil	| Rôle |
|-------/------/
| Git	| Gère l’historique du projet en local |
| GitHub | Stocke ton projet en ligne (sauvegarde + partage) |
| VS Code |	Éditeur de fichiers |
| GitHub Desktop |	Interface simple pour Git (Push/Pull/Commit) |

---

## 2. Installer les outils

✔ Git : https://git-scm.com/

✔ GitHub Desktop : https://desktop.github.com/

✔ VS Code : https://code.visualstudio.com/

✔ Crée un compte GitHub si pas déjà fait

---

## 3. Configurer Git (une seule fois)

Ouvre Git Bash :

git config --global user.name "TonNomGitHub"
git config --global user.email "TonEmailGitHub"


Vérifier :

git config --global --list

---

## 4. Workflow global (méthode pro simple)
Cycle de travail standard

`Pull` (récupérer ce qui existe)

Modifier des fichiers dans VS Code

`git add` (dire quels fichiers garder)

`git commit` (sauvegarder version locale)

`Push` (envoyer sur GitHub)

Règle d’or :

*Toujours `Pull` avant de travailler*

---

##  5. Créer un projet Git local → GitHub
📍 Étapes
1) Créer un dossier
`mkdir mon_projet`
`cd mon_projet`

2) Init Git
`git init`

3) Créer un fichier README

(début minimum du projet)

`echo "# Mon projet" > README.md`

4) Ouvrir dans VS Code sinon ouvrir manuellement VS Code -> File → Open Folder

(si installé dans PATH)

`code .`

5) Ajouter et commit
`git add .`
`git commit -m "Initial commit"`

6) Créer un repo VIDE sur GitHub

Sur GitHub.com :

- New Repository
- nom = mon_projet
- Ne coche rien (pas de README auto)

7) Connecter le local au GitHub
`git remote add origin https://github.com/TONPSEUDO/mon_projet.git`
`git branch -M main`
`git push -u origin main`


✅ Ton projet est maintenant sur GitHub

---

## 6. Cloner un projet GitHub → local
Avec GitHub Desktop

➡️ File → Clone repository
➡️ Coller l’URL
➡️ Choisir un dossier vide

Ou en terminal
`cd /c/Users/TonNom/Documents`   # aller où tu veux
`git clone https://github.com/TONPSEUDO/mon_projet.git`
`cd mon_projet`

Ouvrir dans VS Code par le terminal ou manuellement
`code .`

---

## 7. Modifier et envoyer son travail

Dans VS Code → écrit, modifie.

Dans Terminal :

`git add .`
`git commit -m "Description de la modification"`
`git push`


Dans GitHub Desktop → bouton Commit puis Push

---

🌿 8. Branches simples

Créer une branche :

`git checkout -b dev`

Changer de branche :

`git checkout main`

Voir les branches :

`git branch`

---

💡 9. Commandes Git essentielles (mémo)
|Action	| Commande |
|-------|----------|
|Initialiser Git | git init |
|Voir l’état Git |	git status |
|Ajouter fichiers |	git add . |
|Ajouter message explicatif de la modification | Commit	git commit -m "message" |
|Envoyer sur GitHub | git push |
|Récupérer | git pull |
|Créer branche | git checkout -b nom |
|Changer branche |	git checkout nom |

---

🧼 10. Saut de ligne dans Markdown

- Enter = ligne normale

- deux espaces + Enter = retour visible

- <br> = retour forcé

---

✅ Raccourcis Markdown
| Fonction | Syntaxe | Résultat / Exemple |
|---|---|---|
| Titre H1 | `# Titre` | # Titre |
| Titre H2 | `## Titre` | ## Titre |
| Titre H3 | `### Titre` | ### Titre |
| Texte en gras | `**texte**` | **texte** |
| Texte en italique | `*texte*` | *texte* |
| Gras + italique | `***texte***` | ***texte*** |
| Barré | `~~texte~~` | ~~texte~~ |
| Code inline | `` `code` `` | `code` |
| Bloc de code | <code>```lang<br>code<br>```</code> | Bloc de code |
| Liste à puces | `- Item` | - Item |
| Liste numérotée | `1. Item` | 1. Item |
| Lien | `[texte](https://url)` | [exemple](https://url) |
| Image | `![alt](image.png)` | affiche l'image |
| Citation | `> citation` | > citation |
| Ligne horizontale | `---` | --- |
| Tableau | `|A|B|\n|---|---|\n|1|2|` | Tableau |
| Case à cocher | `- [ ] tâche` | - [ ] tâche |
| Case cochée | `- [x] fait` | - [x] fait |
| Saut de ligne forcé | `Texte␣␣` *(2 espaces)* | (retour à la ligne) |
