## 5. Interactions entre le personnage et les ennemis et Zone de mort ⚔️

- **Saut sur le squelette** :
  - **Condition** : Collision entre `DevoTheDevil` et le squelette lorsque `DevoTheDevil` tombe dessus. 💥
  - **Action** : Changez l’animation du squelette en **"Crumbling Into Bone Pile"** pour le détruire. 🦴💨

- **Collision avec le squelette** :
  - **Condition** : Collision entre le squelette et `DevoTheDevil` par le côté. ❌
  - **Action** : Déclenchez une perte de vie ou affichez l’écran **"Game Over"**. 💔

- **Création et interaction avec la zone de mort** ☠️
  - **Ajout de la zone de mort** :
    - Créez un objet de zone de mort (par exemple nommé `mort`) qui servira de limite fatale pour le joueur, en bas de la scène ou dans des zones spécifiques.
  - **Détection de la collision avec la zone de mort** :
    - **Condition** : Collision entre `DevoTheDevil` et l'objet `mort`.
    - **Actions** :
      - **Supprimez `DevoTheDevil`** pour signaler la fin de la partie.
      - **Affichez l'écran "Lost"** : Changez la scène vers **"Lost"** pour que le joueur sache qu'il a perdu et doit recommencer.
