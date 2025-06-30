# 🎮 Introduction à Unreal Engine

## 🎯 Objectif pédagogique  
Découvrir l’environnement de travail d’Unreal Engine, comprendre la logique d’un niveau de jeu, et apprendre à manipuler les éléments de base dans la scène.

---

## 🔍 Pourquoi utiliser Unreal Engine ?

- Moteur de jeu puissant utilisé par les pros
- Permet de créer des jeux 3D/2D avec ou sans coder (Blueprints)
- Visualisation en temps réel
- Gratuit pour les petits projets ou l'apprentissage

---

## 🖥️ Lancer Unreal Engine

### 1. Ouvrir le **Epic Games Launcher**
> Se connecter avec un compte Epic (création gratuite si nécessaire)

### 2. Créer un projet
- Onglet **Unreal Engine → Library**
- Bouton **Launch**
- Choisir **Games > Blank** ou **Third Person**
- Nom du projet : `MonPremierJeu`
- Activer **Starter Content** ✅
- Créer dans un dossier clair (ex : `C:/StageUnreal`)

---

## 🧭 Interface d’Unreal Engine

### Principales zones à connaître :

| Zone              | Description |
|-------------------|-------------|
| **Viewport**      | Zone principale pour voir et manipuler la scène |
| **Outliner**      | Liste des objets présents dans le niveau |
| **Details**       | Propriétés de l’objet sélectionné |
| **Content Browser** | Bibliothèque de tous les assets (modèles, sons, blueprints…) |
| **Toolbar**       | Actions globales : jouer, sauvegarder, construire, etc. |

---

## 🕹️ Contrôles de la vue 3D

| Action           | Touche / Souris       |
|------------------|------------------------|
| Tourner la caméra | clic droit + souris   |
| Se déplacer       | ZQSD + clic droit     |
| Zoom avant/arrière | molette souris       |
| Sélectionner un objet | clic gauche       |

---

## 🧱 Comprendre la logique de "Niveau" (Level)

- Un **Level** = une scène jouable
- Contient le sol, les objets, les lumières, les personnages, les triggers…
- On peut en avoir plusieurs : menu, niveau 1, niveau 2…

> 🎯 Objectif : être capable de créer une scène simple contenant des objets placés dans l’espace 3D.

---

## 🧪 Activité pratique

1. Créer un cube : `Place Actors > Basic > Cube` → glisser dans la scène
2. Le déplacer (`W`), le faire tourner (`E`), le redimensionner (`R`)
3. Sauvegarder la scène : `File > Save Current Level`
4. Changer le nom du niveau : `Niveau_01`

---

## 🗂️ Bonnes pratiques à transmettre

- Organiser les assets : créer des dossiers (`/Meshes`, `/Materials`, `/Blueprints`, etc.)
- Nommer les objets clairement (`PlayerStart`, `CubePlateforme_01`)
- Sauvegarder fréquemment (`Ctrl + S`)
- Ne pas hésiter à tout tester avec le bouton **Play** dans la barre du haut

---

## ✅ Objectifs atteints

| Savoir-faire                           | Statut |
|----------------------------------------|--------|
| Ouvrir et créer un projet Unreal       | ✅     |
| Comprendre l’interface et s’y repérer  | ✅     |
| Ajouter et manipuler un objet          | ✅     |
| Sauvegarder un niveau                  | ✅     |

---

## 💬 À retenir

> « Le niveau, c’est notre terrain de jeu. L’interface, notre boîte à outils. »

> « Tu n’as rien cassé tant que tu n’as pas supprimé le dossier du projet 😉 »

