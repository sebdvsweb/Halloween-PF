## 1. Configuration du personnage principal et des contrôles 🎮

### 1.1 Comportement de plateforme pour le personnage `DevoTheDevil` 
- Sélectionnez `DevoTheDevil` dans la scène. ✨
- Ajoutez le comportement : Dans les propriétés de l’objet, allez dans **Comportements** > **Ajouter un comportement** > **Objet de plateforme**. 🚀
- Paramétrez les options :
  - **Gravité** : Ajustez pour que `DevoTheDevil` tombe naturellement. 🌪️
  - **Vitesse de marche** : Définissez la vitesse souhaitée pour le mouvement horizontal. 🏃‍♂️💨
  - **Hauteur de saut** : Ajustez selon le niveau de saut souhaité pour votre personnage. 🦘

### 1.2 Comportement de caméra fluide (SmoothCamera) 🎥
- Ajoutez le comportement `SmoothCamera` à `DevoTheDevil` pour que la caméra suive automatiquement le personnage de façon fluide. 🌈 Ce comportement permet d'améliorer l'expérience de jeu en offrant une vue stable et agréable, surtout dans des niveaux étendus ! 🌌

### 1.3 Contrôles de base
- **Aller à droite** :
  - **Condition** : Ajoutez un événement avec la condition **"Touche droite pressée"**. ⏩
  - **Action** : Déplacez `DevoTheDevil` vers la droite en définissant l’**animation de course**. 🎉

- **Aller à gauche** :
  - **Condition** : Ajoutez un événement pour la **touche gauche**. ⏪
  - **Action** : Définissez le **FlipX à "oui"** pour que `DevoTheDevil` regarde dans la bonne direction lorsqu’il se déplace vers la gauche. 🔄

- **Sauter** :
  - **Condition** : Ajoutez un événement pour la **touche Espace**. 🆗
  - **Action** : Simulez une **touche de saut** pour permettre à `DevoTheDevil` de sauter. 🌠
