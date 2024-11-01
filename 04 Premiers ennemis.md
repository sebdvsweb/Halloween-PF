## 4. Ajout et déplacement du squelette ennemi ☠️

Le squelette est programmé pour se déplacer de gauche à droite, changeant de direction lorsqu'il entre en collision avec des objets invisibles placés aux extrémités de son parcours.

### 4.1 Mise en place des points de changement de direction 🔄
- **Création des flèches invisibles** :
  - Placez un objet sans image aux extrémités de la zone de déplacement du squelette (ex. `RightArrowRoundButton` et `LeftArrowRoundButton`).
  - **Astuce** : Dans les propriétés des flèches, décochez **Visible** pour que le joueur ne les voie pas, mais que le squelette puisse interagir avec elles.

### 4.2 Création de la variable de direction pour le squelette 🧭
- **Variable `direction`** : Créez une variable d’objet pour le squelette nommée **direction** avec la valeur initiale `"right"`.

### 4.3 Application des forces et changements de direction 🎯
- **Déplacement à droite** :
  - **Condition** : Si `direction` vaut `"right"` **et** que l’animation actuelle du squelette **n’est pas** `"Crumbling Into Bone Pile"`.
    - 💡 **Explication** : Vérifier que l’animation n’est pas `"Crumbling Into Bone Pile"` empêche le squelette de bouger lorsqu’il est détruit. Par défaut, l’animation est initialisée à `"Standing Idle"` pour qu’il soit immobile au début de la scène.
  - **Actions** :
    - **Appliquez une force** avec un angle de **0° (droite)** et une intensité (par exemple **50**) pour un mouvement continu vers la droite.
    - **Définissez `FlipX` à "Non"** pour que le squelette fasse face à la bonne direction.
    - **Changez l’animation en `"Limping Movement"`** pour animer son déplacement. 🦴

- **Déplacement à gauche** :
  - **Condition** : Si `direction` vaut `"left"` **et** que l’animation du squelette **n’est pas** `"Crumbling Into Bone Pile"`.
    - 💡 **Explication** : Cette condition empêche le squelette de continuer à se déplacer s’il est détruit (animation `"Crumbling Into Bone Pile"`).
  - **Actions** :
    - **Appliquez une force** avec un angle de **180° (gauche)** pour le faire se déplacer dans cette direction.
    - **Définissez `FlipX` à "Oui"** pour qu’il regarde dans cette direction.
    - **Changez l’animation en `"Limping Movement"`** pour animer son déplacement. 👻

### 4.4 Changement de direction aux points d’arrêt 🔄
- **Collision avec la flèche de gauche** :
  - **Condition** : Si le squelette touche `LeftArrowRoundButton`, changez la **direction** à `"right"`.
- **Collision avec la flèche de droite** :
  - **Condition** : Si le squelette touche `RightArrowRoundButton`, changez la **direction** à `"left"`.
