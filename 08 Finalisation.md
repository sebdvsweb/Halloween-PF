## 8. Test final et ajustements ⚙️🧪

![start](https://sebastien-devos.fr/img/codegaming/start.png)

### Écran de démarrage et de fin 🎬
- **Écran de démarrage** : 
  - Créez une scène d’accueil avec un bouton **"Démarrer"** pour lancer le jeu. 🎮 
  - **Événements** :
    - **Condition** : Si le bouton **TransparentButtonWithWhiteBlueBorder** est cliqué. 🖱️
    - **Action** : Passez à la scène **"Level 1"**. 🚪➡️

  - **Animation d'introduction** :
    - **Condition** : Lorsque la scène commence (DepartScene). 🏁
    - **Action** : Changez l'animation de `Skeleton` pour **"Bone Pile Wakeup"** pour ajouter un peu de mystère et de fun ! 🦴✨

![end](https://sebastien-devos.fr/img/codegaming/lost.png)

- **Écran de Game Over** : 
  - Créez une scène qui s'affiche si le joueur perd. 😱
  - **Événements** :
    - **Condition** : Si le bouton **TransparentButtonWithWhiteBlueBorder** est cliqué. 🖱️
    - **Action** : Passez à la scène **"Level 1"** pour recommencer le jeu. 🔄

  - **Animation de Game Over** :
    - **Condition** : Lorsque la scène commence (DepartScene). 🏁
    - **Action** : (Optionnel) Vous pouvez déclencher une animation spéciale pour un squelette ou un autre ennemi pour rendre l'écran de fin encore plus captivant ! 🎃💀

### Bonus : Du son ! 
- Ajouter des effets audio 🔈 à votre jeu pour le rendre plus fun !

### Testez tous les éléments :
- Testez les mouvements, la collecte de clés, les interactions avec les ennemis, et les passages de niveau. 🕹️
- Ajustez les paramètres pour un gameplay amusant et équilibré. ⚖️

🎉 **Félicitations !** Vous avez maintenant toutes les étapes pour créer un jeu de plateforme Halloween en 2D dans GDevelop ! 🥳
