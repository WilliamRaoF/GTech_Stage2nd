# 🧩 Introduction aux Blueprints

## 🎯 Objectif pédagogique

Comprendre le fonctionnement des Blueprints dans Unreal Engine et réaliser des interactions simples sans écrire une seule ligne de code.

---

## 📘 Qu’est-ce que Blueprint ?

Blueprint est le système de **programmation visuelle** d’Unreal Engine.  
Il permet de **créer des logiques de jeu** (mouvements, interactions, déclencheurs...) en reliant des blocs visuels, appelés **nodes**.

> 🎯 C’est l’outil idéal pour **prototyper un jeu rapidement**, même sans savoir coder.

---

## 🧱 Les types de Blueprint

| Type de Blueprint      | Utilisation principale                         |
|------------------------|------------------------------------------------|
| **Actor**              | Objet dans le monde (portes, plateformes...)   |
| **Character / Pawn**   | Joueur ou créature contrôlée                   |
| **Level Blueprint**    | Événements liés au niveau en cours             |
| **Game Mode / GameState** | Règles générales du jeu (victoire, score…) |

---

## 🧭 Interface de Blueprint

Quand vous ouvrez un Blueprint, vous avez :

- **Viewport** : pour voir l’objet (3D)
- **Components** : ajouter des éléments (mesh, son, collision…)
- **Event Graph** : c’est ici qu’on crée la logique visuelle
- **Details Panel** : propriétés du nœud sélectionné

---

## 🧩 Les bases du Graph d’événements

Le **Graph** est constitué de **noeuds** reliés par des **fils** (wires).  
Chaque noeud peut :

- **Déclencher une action** (`Event BeginPlay`, `OnComponentHit`)
- **Exécuter une action** (`Print String`, `Destroy Actor`)
- **Faire une condition** (`Branch`, équivalent d’un "si")

---

## 👣 Exemple simple : afficher un message au démarrage

### Étapes :

1. Ouvrir le **Level Blueprint** :  
   `Menu > Blueprints > Open Level Blueprint`

2. Ajouter ce graphe :

- `Event BeginPlay` → `Print String`
- Entrer un texte : `"Bienvenue dans le jeu !"`

3. Appuyer sur **Play**

🎉 Le message s'affiche à l'écran au lancement !

---

## 🚪 Exemple 2 : ouvrir une porte au contact

### Objectif :
Créer un Blueprint Actor représentant une porte qui **disparaît** quand on entre en collision.

### Étapes :

1. `Add > Blueprint Class > Actor` → nommer `BP_Door`
2. Ouvrir BP_Door :
   - Ajouter un **Cube** (Static Mesh)
   - Ajouter un **Box Collision**
   - Dans le Graph :  
     - `OnComponentBeginOverlap (Box)` → `Destroy Actor`

3. Glisser l’acteur dans la scène
4. Jouer : quand le joueur touche la porte, elle disparaît

---

## 🔁 Bonus : créer un interrupteur

1. Ajouter un **Trigger Box** dans le niveau
2. Ouvrir le **Level Blueprint**
3. Clic-droit dans le graph, ajouter `OnActorBeginOverlap (TriggerBox)`
4. Relier à une action comme `Open Door`, `Print`, etc.

---

## ✅ Objectifs atteints

| Compétence                                         | Statut attendu |
|----------------------------------------------------|----------------|
| Ouvrir un Level Blueprint                          | ✅             |
| Créer un événement `Begin Play`                    | ✅             |
| Ajouter une action `Print String`                  | ✅             |
| Créer un Blueprint Actor avec collision            | ✅             |
| Comprendre la logique **déclencheur → action**     | ✅             |

---

## 💬 À retenir

> "Blueprint, c’est comme un Lego géant : chaque bloc a une fonction. En les combinant, on peut faire des jeux entiers sans jamais taper une ligne de code."

> "Commencez simple : une action, une cause, un effet."
