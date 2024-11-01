## 7. Ajout du trampoline et de l'ennemi mouche (Niveau 2) 🪄🦘🐝

### 7.1 Trampoline
- **Ajout du trampoline** :
  - Dans le niveau 2, ajoutez un objet trampoline à l’endroit souhaité. 🎢
  - **Condition** : Détection d'une collision entre `DevoTheDevil` et le trampoline. 🤸
  - **Actions** :
    - Changez l’animation du trampoline pour **"Jump"** lors de la collision. 🎊
    - Permettez à `DevoTheDevil` de sauter en simulant une pression sur la touche de saut avec **SimulateJumpKey**. 🚀
    - Réglez la vitesse de saut à **1200** pour un rebond puissant. ⚡
    - Après une seconde, revenez à l'animation **"Idle"**. ⏱️

### 7.2 Ennemis mouches
- **Ajout d'un ennemi mouche** :
  - Ajoutez un objet représentant la mouche (`FlyEnemy`) dans le niveau 2. 🐝
  - Configurez le mouvement de la mouche pour qu'elle se déplace de haut en bas ou en zigzag. 🌀
  - Assurez-vous que si `DevoTheDevil` entre en collision avec la mouche, cela déclenche une perte de vie. 💔
