# correspondenceDHI

1. Trouver et eleminer les doublets dans les index avec OpenRefine
   1. Doublets : Nom - Facet - Text facet -> name count
   2. Noms écrits de manière similaire : Nom - Edit cells - Cluster and edit -> jouer avec "Method" et "Keying Function"
   - Identifier les mentions des mêmes persons -> "Merge selected & Close"
   - Supprimer les nouvelles doublets

2. Enrechir les Persones/lieux avec Geodata
   1. Créer une nouvelle colonne avec les Json/XML des bases de données normatives
      - **Geocodage** : Tutoriel : https://opensas.wordpress.com/2013/06/30/using-openrefine-to-geocode-your-data-using-google-and-openstreetmap-api/
      - Create column :  "https://nominatim.openstreetmap.org/search?q="+(cells["Name of Column"].value)+"&format=json"
      - Create column for lat and long :  
         value.parseJson()[0].lat
         value.parseJson()[0].lon
   3.  
 
3. Preparer les index pour des Graphes - **Edges:** Index_of_persons, of_places, of works
   1. Séparer les ID des lettres écrites dans un champ : Renvoi... - Edit cells - Split multi-valued cells
   2. Remplir les lignes nouvellement créées avec les noms et les ID des personnes/lieux/œuvres : Nom - Edit cells - Fill down 
  
