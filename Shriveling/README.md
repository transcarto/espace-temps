
# Espace-temps

## Ratatinement / Shriveling

[Shriveling world](https://theworldisnotflat.github.io/shriveling_world/marks/index) est une application conçue pour créer des images en trois dimensions de l'espace-temps géographique, reposant sur le principe d'un ratatinement (*shriveling*) de l'espace

### TP de prise en main

1. Ouvrir l'URL: https://github.com/theworldisnotflat/shriveling_world
2. Cliquer sur le lien de l'application: https://theworldisnotflat.github.io/shriveling_world/marks/index
3. Cliquer sur le bouton *Application*. L'interface se présente à vous avec :
   * des contrôles à droite
   * une liste de jeux de données à gauche
   * les liens vers le site web en haut (survoler pour les faire apparaître)
     * l'aide dans le menu *User Doc*
   * un bouton "save scene" en bas

4. Charger un jeu de données :
   * Cliquer sur un jeu de données, attendre
   * Alternativemement, sélectionner les 6 fichiers d'un jeu de données, et faites les glisser puis déposer dans la fenêtre de l'application, attendre
     * La composition d'un jeu de données est [expliquée ici](https://theworldisnotflat.github.io/shriveling_world/marks/usrdoc/create_dataset)
     * Un jeu de données décrit un réseau de transport (villes, réseau, vitesses) et d'un fichier de contours géographiques

5. Manipuler la molette de la souris (voir [navigation](https://theworldisnotflat.github.io/shriveling_world/marks/usrdoc/basic_usage_tutorial/#navigation) dans l'[aide](https://theworldisnotflat.github.io/shriveling_world/marks/usrdoc/basic_usage_tutorial/)) pour obtenir une vue satisfaisante, qui révèle le relief
   * **Zoom** = Molette
   * **Rotation** = Clic gauche + mouvement de la souris
   * **Translation** = Clic droit + mouvement de la souris

6. Affichage des cônes
   * Clic sur "cones"
   * coneStep = niveau de définition graphique des cônes, pour la valeur 1 le cône est décrit par 360 triangles, pour la valeur 10, 36 triangles (pése sur la taille du fichier de sortie)
     * valeur recommandée 1
   * withLimits = découpe les cônes au contour géographique (comporte des erreurs, à réaliser dans Blender)
     * décocher
   * Transparence

7. Affichage des arcs
   * Clic sur "curves"
   * number of points = niveau de définition graphique des arcs (pése sur la taille du fichier de sortie)
      * valeur 1 = lignes droites
      * valeur 2 = lignes brisées (génère des artefacts dans Blender, [erreur connue](https://github.com/theworldisnotflat/shriveling_world/issues/159))
      * valeur 50 et + = courbes lisses
   * Couleur (attention, quelques erreurs dans l'affichage, reproduire la manipulation si les couleurs se perdent)
   * Transparence

8. Légende
   * La légende figure la pente générale des cônes, le mode routier, rapporté au mode le plus rapide sur l'esapce considéré
   * Survoler la légende permet d'afficher les vitesses et les pentes du modèle

9. Exploration du temps historique
   * Suivant les données incluses dans les fichiers *transport_mode_speed* et *network* 

10. Exportation
   * Une copie d'écran permet de produire une image à habiller por créer une carte
   * Le bouton *Save scene* exporte dans le format
