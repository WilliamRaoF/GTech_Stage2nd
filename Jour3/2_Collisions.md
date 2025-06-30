# 🚶 Premiers tests : déplacement & collisions

## 🎯 Objectif pédagogique  
Tester le déplacement du personnage dans Unreal Engine, comprendre le fonctionnement des collisions, et créer un petit parcours d'obstacles.

---

## 🧍 Déplacement de base (template Third Person)

### Étapes :

1. **Ouvrir un projet Unreal avec le template "Third Person"**
2. Lancer le jeu via le bouton **Play**
3. Utiliser les touches **ZQSD** ou **flèches directionnelles** pour bouger
4. Tester le **saut** avec la barre espace

> ✅ Le personnage est déjà contrôlable grâce au système Blueprint fourni par Unreal dans ce template.

---

## 📦 Comprendre le rôle de Player Start

### C’est quoi ?
- Un **point de départ** pour le joueur
- À placer pour définir où le joueur apparaît

### Ajouter un Player Start :
1. `Place Actors > All Classes > Player Start`
2. Le positionner sur le sol avec `W`
3. Supprimer ou déplacer les anciens si besoin

> ⚠️ Sans Player Start, le jeu peut ne pas démarrer correctement.

---

## 🔁 Tester les collisions

### Qu’est-ce qu’une collision ?
- Empêche un objet d’en traverser un autre
- Détecte le contact entre joueur et décor

### Exemples d’objets avec collision :
- Cube, sol, mur → **Collision par défaut**
- Textures, décor décoratif → parfois **pas de collision**

### Tester :
1. Ajouter des cubes, sphères, murs
2. Lancer le jeu avec **Play**
3. Vérifier si le personnage **rebondit** ou **traverse** l’objet

---

## ⚙️ Paramètres importants de collision

1. Sélectionner un objet
2. Onglet **Details > Collision**
   - **Collision Presets** : choisir **BlockAll** (bloque tout)
   - **Generate Overlap Events** : active les déclencheurs

### Types courants :
| Type           | Description                                 |
|----------------|---------------------------------------------|
| BlockAll       | Empêche tout de passer                      |
| OverlapAll     | N'empêche pas, mais détecte le contact      |
| NoCollision    | Ignore totalement les collisions            |

---

## 🧱 Créer un parcours simple

### Objectif :
Construire une mini-arène de test avec :
- Un sol
- Des murs ou cubes à éviter
- Un ou plusieurs objets à traverser ou sauter

### Étapes :
1. Placer un sol (`Geometry > Box` ou `Floor`)
2. Ajouter des cubes, rampes ou obstacles
3. Tester les déplacements
4. Ajuster la **taille et hauteur des éléments** si besoin

---

## ✅ Objectifs atteints

| Compétence                              | Statut attendu      |
|-----------------------------------------|---------------------|
| Le joueur peut se déplacer              | ✅                  |
| Le joueur ne tombe pas dans le vide     | ✅                  |
| Les objets solides bloquent le joueur   | ✅                  |
| Un parcours test est jouable            | ✅                  |

---

## 💡 Astuces

- Toujours vérifier que vos éléments sont bien **au-dessus du sol** dans le viewport
- Pour "attraper" un objet : activer le **snap au sol (Alt + clic)** ou aligner avec `End`
- Pour supprimer un élément trop petit à attraper → clic droit → Delete

---

## 💬 À retenir

> « Pas de fun sans contrôle ! Si ton joueur glisse ou traverse tout, ce n’est plus un jeu 😉 »

> « Une collision bien réglée, c’est la base du gameplay. »

