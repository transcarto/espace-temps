
# Espace-temps

## Ratatinement / Shriveling

[Shriveling world](https://theworldisnotflat.github.io/shriveling_world/marks/index) est une application conçue pour créer des images en trois dimensions de l'espace-temps géographique, reposant sur le principe d'un ratatinement (shriveling) de l'espace

### TP de prise en main

1. Ouvrir l'URL: https://github.com/theworldisnotflat/shriveling_world
2. Cliquer sur le lien de l'application: https://theworldisnotflat.github.io/shriveling_world/marks/index
3. Cliquer sur le bouton 'Application'. L'interface se présente à vous avec :
   * des contrôles à droite
   * une liste de jeux de données à gauche
   * les liens vers le site web en haut (survoler pour les faire apparaître)
      * l'aide dans le menu "User Doc"
   * un bouton "save scene" en bas

4. Charger un jeu de données :
   * Cliquer sur un jeu de données, attendre
   * Alternativemement, sélectionner les 6 fichiers d'un jeu de données, et faites les glisser puis déposer dans la fenêtre de l'application
      * La composition d'un jeu de données est [expliquée ici](https://theworldisnotflat.github.io/shriveling_world/marks/usrdoc/create_dataset)
      * Un jeu de données décrit un réseau de transport (villes, réseau, vitesses) et d'un fichier de contours géographiques
5. Manipuler la molette de la souris (voir [navigation](https://theworldisnotflat.github.io/shriveling_world/marks/usrdoc/basic_usage_tutorial/#navigation) dans l'[aide](https://theworldisnotflat.github.io/shriveling_world/marks/usrdoc/basic_usage_tutorial/)) pour obtenir une vue satisfaisante, qui révèle le relief
   * Zoom = Molette
   * Rotation = Clic gauche + mouvement de la souris
   * Translation = Clic droit + mouvement de la souris
6. Affichage des cônes
   * Clic sur "cones"
   * coneStep = fixe le niveau de définition graphique des cônes, pour la valeur 1 le cône est décrit par 360 triangles, pour la valeur 10, 36 triangles
      * valeur recommandée 1
   * withLimits = découpe les cônes au contour géographique (comporte des erreurs, à réaliser dans Blender)
      * décocher

7. Affichage des arcs
