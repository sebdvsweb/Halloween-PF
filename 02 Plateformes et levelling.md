## 2. Ajout de plateformes mobiles et fixes 🏞️

![Plateformes](https://sebastien-devos.fr/img/codegaming/pixel-platformer.png)

### Plateformes fixes
- Placez votre personnage sur une plateforme centrale à la scène de base. 🌄
- Placez ensuite les plateformes statiques pour créer le parcours du personnage tout autour. 🌄
- Utilisez de préférence les plateformes `Tile 8`, `Tile 9`, `Tile 11`, `Tile 17`.
- N'hésitez pas ajouter des élements de décors - buissons, et autres !

### Plateformes mobiles
- Ajoutez une plateforme mobile (par exemple `Platform1`) et allez dans **Propriétés** > **Comportements**. 📏
- Ajoutez le comportement **RectangleMovement** : Choisissez les options pour qu'elle se déplace horizontalement ou verticalement. ⬅️➡️
- Définissez la distance de déplacement et la vitesse pour créer un mouvement fluide. 🌊

### Étendre la scène
- Augmentez la largeur de la scène pour créer un niveau plus vaste avec un effet de scrolling horizontal automatique, grâce au comportement automatique de la caméra. 📸🌌
- Pour cela, n'hésitez pas à dupliquer vos fonds et à les coller les uns à côté des autres. Pour les aligner, vérifier leur coordonnées en Y.
- Continuer à agrémenter le parcours de plateformes fixes et/ou mouvantes.  ⬅️➡️

N'oubliez pas de gérer si besoin l'option `z-index` de vos objets pour gérer les différentes couches de profondeurs.

