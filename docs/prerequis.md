---

````markdown
# ⚙️ Prérequis & Installation

## 🎯 Objectif
Avant de commencer les mini-projets du TP *Godot → HAARP RTS*, il faut préparer ton environnement de développement sur macOS.

---

## 🧰 1️⃣ Logiciels indispensables

### 🟩 Godot Engine 4.x
Le moteur principal pour créer les jeux 2D et 3D.

- Télécharge depuis : [https://godotengine.org/download](https://godotengine.org/download)
- Ou installe via Homebrew :
  ```bash
  brew install --cask godot
````

💡 *Conseil : place Godot dans ton dossier “Applications” pour y accéder facilement.*

---

### 💻 Visual Studio Code

Ton éditeur de code pour GDScript, Python ou Markdown.

* Télécharge depuis : [https://code.visualstudio.com](https://code.visualstudio.com)
* Ou installe via Homebrew :

  ```bash
  brew install --cask visual-studio-code
  ```

#### Extensions recommandées :

* **Godot Tools** : intégration complète Godot + VS Code
* **Markdown All in One** : pour rédiger les fiches du TP
* **GitLens** : visualiser les commits Git
* **Material Icon Theme** *(optionnel, pour une arborescence claire)*

---

### 🧱 Git

Indispensable pour versionner ton travail et collaborer via GitHub.

```bash
brew install git
```

Vérifie l’installation :

```bash
git --version
```

Configure ton identité :

```bash
git config --global user.name "Siegfried Sekkai"
git config --global user.email "ton_email@exemple.com"
```

---

## 🌐 2️⃣ Créer ton dépôt GitHub

1. Connecte-toi sur [https://github.com](https://github.com)
2. Crée un nouveau dépôt nommé :

   ```
   godot-tp-haarp
   ```
3. Coche l’option **“Initialize this repository with a README”**
4. Clone ton dépôt localement :

   ```bash
   git clone https://github.com/<ton_nom>/godot-tp-haarp.git
   ```
5. Crée les dossiers :

   ```bash
   mkdir -p docs/steps assets scripts
   ```

---

## 🧩 3️⃣ Organisation du projet

Chaque mini-jeu aura :

```
/SquareHero/
    ├── project.godot
    ├── scenes/
    ├── scripts/
    ├── assets/
    └── README.md
```

La documentation associée sera dans :

```
/docs/steps/step1_squarehero.md
```

---

## 🧠 4️⃣ Vérification rapide

Lance ces commandes dans ton terminal :

```bash
godot --version
code --version
git --version
```

Si tu vois une version pour chacun → ton environnement est prêt ✅

---

## 💡 5️⃣ (Optionnel) Automatiser l’environnement

Tu peux créer un fichier `setup.sh` pour tout installer en un clic :

```bash
#!/bin/bash
brew install --cask godot visual-studio-code
brew install git
code --install-extension geequlim.godot-tools
code --install-extension yzhang.markdown-all-in-one
code --install-extension eamodio.gitlens
```

Rends-le exécutable :

```bash
chmod +x setup.sh
```

Et exécute :

```bash
./setup.sh
```

---

## ✅ Résumé des prérequis

| Outil      | Rôle                | Installation                             |
| ---------- | ------------------- | ---------------------------------------- |
| Godot      | Moteur de jeu       | `brew install --cask godot`              |
| VS Code    | Éditeur de code     | `brew install --cask visual-studio-code` |
| Git        | Gestion de versions | `brew install git`                       |
| GitHub     | Hébergement du code | [github.com](https://github.com)         |
| Extensions | Productivité        | Godot Tools, Markdown, GitLens           |

---

> 🧭 **Prochaine étape :** [Étape 1 — Square Hero](./steps/step1_squarehero.md)

```
