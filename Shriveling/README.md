
# Ratatinement / Shriveling

[Shriveling world](https://theworldisnotflat.github.io/shriveling_world/marks/index) est une application conçue pour créer des images en trois dimensions de l'espace-temps géographique, reposant sur le principe d'un ratatinement (*shriveling*) de l'espace géographique. Le projet comporte un [site github](https://github.com/theworldisnotflat/shriveling_world), un [forum d'utilisateurs](https://github.com/theworldisnotflat/shriveling_world/discussions) ainsi qu'un [blog scientifique](https://timespace.hypotheses.org/).

## Module A Prise en main

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

8. Modifier l'éclairage de la scene
   * *Light intensity*
   * Position de la source lumineuse: *x*, *y*, *z*
9. Légende
   * La légende figure la pente générale des cônes, le mode routier, rapporté au mode le plus rapide sur l'esapce considéré
   * Survoler la légende permet d'afficher les vitesses et les pentes du modèle

10. Exploration du temps historique
   * Suivant les données incluses dans les fichiers *transport_mode_speed* et *network*, il est possible de définir la date de référence:
     * Clic sur *Generalities*
     * Faire glisser *year*

11. Exportation
    * Une copie d'écran permet de produire une image à habiller por créer une carte
    * Le bouton *Save scene* exporte dans le format *obj* reconnu par Blender
      * Blender permet de prendre la main de manière complète sur les paramètres visuels de l'image finale

## Module B TP sortie France

1. Cliquer sur le jeu de données *France*
2. Rendre invisibles les routes (*road*)
3. Colorer les TGV en rouge (*HST*)
4. Mettre la transparence de TGV à zéro (pour maximiser leur visibilité)
5. Fixer une orientation permettant de visualiser le relief
6. Agir sur la lumière
7. Effectuer une copie d'écran

## Module C Blender

L'utilisation de Blender avec les données Shriveling est décrite dans [ce tutoriel](https://theworldisnotflat.github.io/shriveling_world/marks/usrdoc/blender_tutorial). Le TP se décompose ainsi:
1. _Export scene_ depuis __Shriveling world__
2. Import scene in Blender
3. Test and correct normals
4. Fusionner les cônes
5. Supprimer le noeud des courbes situé au centre de la terre
6. Convertir les arcs en _curves_
7. Ajuster l'épaisseur des _curves_
8. Définir le matériau des _curves_
9. Découper les cônes à la frontière
10. Préparer le rendering
11. Mettre en oeuvre la HDRI
12. Mettre en place la caméra
13. Effectuer un rendu F12 (à confirmer)

## Module D Adapter un jeu de données : Isère

Les jeux de données de l'Isère ont été produit avec [QGIS](https://www.qgis.org/fr/site/) en suivant [les instructions indiquées ici](https://github.com/theworldisnotflat/shriveling_world/blob/master/markdown/usrdoc/create_dataset_from_scratch.md) et aussi [ici](https://theworldisnotflat.github.io/shriveling_world/marks/usrdoc/create_dataset).

Deux jeux de données sont disponibles:
* [Réseau à 512 noeuds](https://github.com/transcarto/espace-temps/tree/main/Shriveling/38) (les 512 communes de l'Isère)
* [Réseau à 48 noeuds](https://github.com/transcarto/espace-temps/tree/main/Shriveling/38_sup5000) (communes de plus de 5000 habitants)

### Télécharger les données

Depuis [la racine du GitHub espace-temps](https://github.com/transcarto/espace-temps) cliquer sur _Code_ puis _Download ZIP_

### Modifier les vitesses

### Modifier la liste des villes
### Modifier le réseau

## Module E Créer un jeu de données
