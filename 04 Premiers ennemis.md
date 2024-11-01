## 4. Ajout et déplacement du squelette ennemi ☠️

![Skeleton](https://sebastien-devos.fr/img/codegaming/skeleton.png)

Le squelette se déplace de gauche à droite en changeant de direction au contact de flèches invisibles. 🔄

### 4.1 Mise en place des points de changement de direction 🔄
- **Création des flèches invisibles** :
  - Placez un objet sans image aux extrémités de la zone de déplacement du squelette (ex. `RightArrow` et `LeftArrow`). 🏹
  - Dans les propriétés des flèches, décochez **Visible**. 👀❌

### 4.2 Création de la variable de direction pour le squelette 🧭
- **Variable direction** : Créez une variable d’objet pour le squelette nommée **direction** avec la valeur initiale **"right"**. ➡️

### 4.3 Application des forces et changements de direction 🎯
- **Déplacement à droite** :
  - **Condition** : Si **direction** vaut **"right"**. 🔜
  - **Actions** :
    - Appliquez une force avec un angle de **0°** (droite) et une intensité (par exemple **50**) pour un mouvement continu vers la droite. 💨
    - Définissez **FlipX à "Non"** pour que le squelette fasse face à la bonne direction. 👻

- **Déplacement à gauche** :
  - **Condition** : Si **direction** vaut **"left"**. 🔙
  - **Actions** :
    - Appliquez une force avec un angle de **180°** pour le faire se déplacer vers la gauche. ⬅️
    - **FlipX à "Oui"** pour qu’il regarde dans cette direction. 👀

### 4.4 Changement de direction aux points d’arrêt 🔄
- **Collision avec la flèche de gauche** : Si le squelette touche **LeftArrow**, changez **direction** à **"right"**. ↩️
- **Collision avec la flèche de droite** : Si le squelette touche **RightArrow**, changez **direction** à **"left"**. ↪️
