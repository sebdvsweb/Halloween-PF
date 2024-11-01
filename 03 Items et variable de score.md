## 3. Système de collecte de clés 🗝️ et gestion du score 📈

![Key](https://sebastien-devos.fr/img/codegaming/key.png)

### 3.1 Score
- Dans la section **Variables de scène**, créez une variable **score** pour enregistrer le nombre de clés collectées par le joueur. 🏅

### 3.2 Collecte des clés
- **Condition** : Collision entre `DevoTheDevil` et une clé. 🎯
- **Actions** :
  - Supprimez l’objet **Key**. ❌
  - Incrémentez la variable **score** de 1. ➕
  - **Affichez le score** : Créez un texte sur la scène qui sera mis à jour en fonction de la variable score. 📝
