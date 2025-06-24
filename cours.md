# Cours Complet sur Scratch

## Introduction

Scratch est un langage de programmation visuel développé par le MIT, destiné principalement aux débutants. Il utilise un système de blocs à assembler pour créer des jeux, animations, et histoires interactives sans avoir besoin de taper du code.

Lien : [https://scratch.mit.edu](https://scratch.mit.edu)

---

## Objectifs du cours

- Comprendre l’environnement de Scratch
- Manipuler les blocs de base (mouvement, événements, contrôle, etc.)
- Créer un petit projet interactif
- Apprendre les bases de la programmation : séquence, boucle, condition, variable

---

## 1. L’interface de Scratch

| Élément | Description |
|--------|-------------|
| Scène | Zone où les sprites évoluent |
| Sprites | Objets/personnages à programmer |
| Zone de script | Endroit où on assemble les blocs |
| Bibliothèques | Pour ajouter des sprites, décors, sons |

---

## 2. Catégories de blocs

| Couleur | Catégorie | Description |
|--------|-----------|-------------|
| Bleu | Mouvement | Déplace les sprites |
| Violet | Apparence | Change l’apparence ou affiche du texte |
| Orange | Contrôle | Boucles, conditions |
| Jaune | Événements | Déclenche les scripts |
| Vert | Opérateurs | Mathématiques, logique |
| Bleu clair | Capteurs | Souris, contact, touches, etc. |
| Orange clair | Variables | Créer et utiliser des valeurs |

---

## 3. Blocs fondamentaux

### Départ du programme

```scratch
quand drapeau vert cliqué
````

### Répétition

```scratch
répéter 10 fois
    avancer de 10
```

### Conditions

```scratch
si <touche espace pressée> alors
    jouer le son "pop"
```

### Variable

```scratch
mettre score à 0
ajouter 1 à score
```

---

## 4. Projet guidé : Jeu de clic

### Objectif

Le joueur doit cliquer sur un sprite qui change de position pour gagner des points.

### Étapes

1. Ajouter un sprite (ex: pomme)
2. Créer une variable : `score`
3. Ajouter ce script au sprite :

```scratch
quand drapeau vert cliqué
mettre score à 0
répéter indéfiniment
    aller à x: (aléatoire entre -200 et 200) y: (aléatoire entre -150 et 150)
    attendre 1 seconde
```

```scratch
quand ce sprite est cliqué
ajouter 1 à score
jouer le son "pop"
```

---

## 5. Concepts clés en programmation

| Concept   | Description                                 | Exemple                         |
| --------- | ------------------------------------------- | ------------------------------- |
| Séquence  | Exécuter les blocs dans l’ordre             | Avancer → Tourner               |
| Boucle    | Répéter une action                          | Répéter indéfiniment            |
| Condition | Faire une action si une condition est vraie | Si \<touche pressée> alors...   |
| Variable  | Stocker une valeur modifiable               | Score, temps, vies              |
| Événement | Déclenche un script                         | Clic sur sprite, touche pressée |

---

## 6. Exercices pratiques

### Exercice 1 : Animation simple

Créer un sprite qui se déplace en boucle et change de costume.

### Exercice 2 : Cible mobile

Le sprite se déplace aléatoirement, et on gagne 1 point à chaque clic.

### Exercice 3 : Quiz interactif

Pose une question et réagit en fonction de la réponse (avec `demander` et `réponse`).

---

## 7. Pour aller plus loin

* Utiliser les listes pour stocker plusieurs éléments
* Créer des clones pour faire apparaître plusieurs objets identiques
* Ajouter des niveaux, un chronomètre, ou des sons personnalisés

---

## Conseils pédagogiques

* Travailler en petits projets, un objectif à la fois
* Favoriser l’expérimentation libre
* Réviser régulièrement les concepts vus
* Partager et observer les projets des autres sur Scratch

---

## Ressources utiles

* Tutoriels officiels : [https://scratch.mit.edu/ideas](https://scratch.mit.edu/ideas)
* Scratch en classe : [https://scratch.mit.edu/educators](https://scratch.mit.edu/educators)
* YouTube : Recherchez "Scratch débutant" pour des vidéos pratiques


