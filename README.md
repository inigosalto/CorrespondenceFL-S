# correspondenceDHI

1. Trouver et eleminer les doublets dans les index avec OpenRefine
* 1.1 Doublets : Nom - Facet - Text facet -> name count
 1.2 Noms écrits de manière similaire : Nom - Edit cells - Cluster and edit -> jouer avec "Method" et "Keying Function"
                                        Identifier les mentions des mêmes persons -> "Merge selected & Close"
2. Enrechir les Persones/lieux avec Geodata
 2.1
 
3. Preparer les index pour des Graphes - **Edges:** Index_of_persons, of_places, of works
 3.1 Séparer les ID des lettres écrites dans un champ : Renvoi... - Edit cells - Split multi-valued cells
 3.2 Remplir les lignes nouvellement créées avec les noms et les ID des personnes/lieux/œuvres : Nom - Edit cells - Fill down
 
 
  
