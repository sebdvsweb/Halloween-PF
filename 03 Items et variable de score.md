## 3. Système de collecte de clés 🗝️ et gestion du score 📈

![Key](https://sebastien-devos.fr/img/codegaming/key.png)

### 3.1 Création et mise à jour du score
1. **Variable de score** :
   - Dans la section **Variables de scène**, créez une variable appelée **score** pour enregistrer le nombre de clés collectées par le joueur.
2. **Affichage du score** :
   - Ajoutez un objet **Texte** sur la scène, nommé par exemple `ScoreDisplay`, pour afficher le score en haut de l’écran.
   - Créez un nouveau calque `UI` et placez-y le score, sur la scène de base.
   - Dans les actions d’événement, utilisez cette commande pour mettre à jour le texte du score en fonction de la variable `score` :

     ```plaintext
     Score : " + ToString(Variable(score))
     ```

   - 💡 **Explication** : Le texte `"Score : "` est combiné à la valeur de la variable `score` en utilisant `ToString(Variable(score))`, ce qui convertit la variable numérique en texte. Ainsi, chaque fois que le joueur collecte une clé, le score s’affiche et se met à jour automatiquement avec le nombre actuel de clés collectées. 🎉

### 3.2 Collecte des clés 🗝️
- **Condition** : Collision entre `DevoTheDevil` et une clé.
- **Actions** :
  - **Supprimez l’objet `Key`** pour simuler la collecte de la clé.
  - **Incrémentez la variable `score` de 1** pour chaque clé collectée.
  - **Mettez à jour le texte du score** en utilisant l’action expliquée ci-dessus pour que le score affiché reflète immédiatement la collecte de la nouvelle clé.
