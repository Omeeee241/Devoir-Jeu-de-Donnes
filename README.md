## Examen de datavizualisation

# Le niveau de délinquance en France et aux Etats-Unis 

# Sommaire
1. Introduction 
2. Choix & présentation des données 
3. Visualisations et analyse  
4. Conclusion 


# Introduction 
Les crimes et délits sont des fléaux de société. Chaque jour, des infractions, plus dangereuses les unes que les autres sont commises dans le monde. Ici, nous allons voir à l'aide de deux jeux de données, des infractions de plusieurs types commis et recensés en France durant l'année 2016 et aux Etats-Unis entre 2000 et 2018. Même si ces informations ne répertorient pas l'ensemble des crimes qui peuvent exister, ils nous montreront tout de même, approximativement, puisque certains délits échappent à la police, ce qu'il en est du taux de violence concernant ce genre de délits dans ces deux pays.  


# Présentation des données 
Pour pouvoir mesurer plus ou moins ce niveau de violence, nous avons choisi les jeux de données qui suivent : 
<iframe src="https://data.opendatasoft.com/explore/embed/dataset/crimes-et-delits-enregistres-par-les-forces-de-securite-en-2016-par-departement@public/table/?location=4,43.96119,3.33984&basemap=jawg.streets&static=false&datasetcard=false" width="600" height="450" frameborder="0"></iframe>

Ces informations fournies par le Service statistique ministériel de la sécurité intérieure, comptabilise le nombre d'infractions commises sur les territoires des différentes communes françaises. On y retrouve également l'effectif de la population ainsi que le nombre de logements. 

<iframe src="https://data.opendatasoft.com/explore/embed/dataset/fbi-crime-data-test@cityofsalinas/table/?&static=false&datasetcard=false" width="600" height="450" frameborder="0"></iframe>

  Ces informations proviennent du bureau fédéral d'enquête du FBI. Le jeu de données concernant les Etats-Unis a été nettoyé à l'aide d'OpenRefine dans le but de ressortir les informations qui nous interessaient vraiment (les modifications se trouvent en fin de page)

# Visualisations et analyse  

Cette carte interactive permet de visualiser en cliquant sur un departement la totalité des informations du jeu de données, elle est pratique pour cnsulter les données tout en visualisant bien où se situe tel ou tel département (nord, sud, est, ouest), mais ne permet pas de voir concrètement où le niveau de violence est plus élevé en fonction des différents délits.  

<iframe frameborder="0" width="800" height="600" src="https://data.opendatasoft.com/map/embed/carte0/?&static=false&scrollWheelZoom=false"></iframe>

C'est pourquoi nous avons choisi de présenter également ce graphique qui permet donc de visualiser le taux d'infraction selon le type et le département de manière plus claire. 

<iframe title="Délits et crimes par types dans les communes françaises" aria-label="Barres empilées" id="datawrapper-chart-bSB9a" src="https://datawrapper.dwcdn.net/bSB9a/1/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="2634"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",(function(e){if(void 0!==e.data["datawrapper-height"]){var t=document.querySelectorAll("iframe");for(var a in e.data["datawrapper-height"])for(var r=0;r<t.length;r++){if(t[r].contentWindow===e.source)t[r].style.height=e.data["datawrapper-height"][a]+"px"}}}))}();</script>

Aux vues de ce graphique, il est indéniable que Paris était la ville la plus touchée par le Vols sans violence contre des personnes donc tres certaines de pickpocket. Pour une ville touristique de cette envergure cela s'explique. Dans les Bouches du Rhone, les cambriolages et vols de voitures sont beaucoup plus nombreux qu'ailleurs. 
Une infraction reste une infraction mais on peut voir tout de même que cela reste minime comparé à certains pays dans lesquels ce genre de comportements est presqu'une habitude. Aussi par raaport au nombre d'habitant cela rest une fois de plus minime. 

Maintenant nous allons voir le cas des Etats unis à l'aide du graphique suivant :  
  
 <iframe title="Nombres de délits et crimes aux Etats-Unis entre 2000 &amp;amp; 2018" aria-label="Anneau de choix" id="datawrapper-chart-B0jfw" src="https://datawrapper.dwcdn.net/B0jfw/1/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="631"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",(function(e){if(void 0!==e.data["datawrapper-height"]){var t=document.querySelectorAll("iframe");for(var a in e.data["datawrapper-height"])for(var r=0;r<t.length;r++){if(t[r].contentWindow===e.source)t[r].style.height=e.data["datawrapper-height"][a]+"px"}}}))}();</script>
  
 Les Etats-Unis comptent une population bien plus élévée que celle de la France et l'on remarque que les crimes contre des biens sont les plus nombreux sur ce territoire. En 18 ans, tous les délits concernés sont resté presque constants, ils ont certes diminuer mais de peu en général, aussi 
  
  
# Conclusion 
  Pour conclure, on peut voir qu'entre la France et les Etats-Unis il y'a une grand pas. L'approche pour visualiser les données n'est pas la même pour les deux jeux car pour l'un, les infractions sont comptabilisées par communes et pour l'autre elles sont comptabilisées nationalement c'est à dire de manière globale mais même en additionnant les données de chaques communes on atteindrait des taux supérieurs ou égaux à ceux des Etats-Unis. On peut aussi malheureusement constater que la délinquance n'est pas un fait qui est prêt de s'arreter. 
  
  
  
  
  ### Modifications OpenRefine
  [
  {
    "op": "core/column-removal",
    "columnName": "Population1",
    "description": "Remove column Population1"
  },
  {
    "op": "core/column-removal",
    "columnName": "Rape\n(revised \ndefinition)3",
    "description": "Remove column Rape\n(revised \ndefinition)3"
  },
  {
    "op": "core/column-removal",
    "columnName": "Rape\n(revised \ndefinition) \nrate3",
    "description": "Remove column Rape\n(revised \ndefinition) \nrate3"
  },
  {
    "op": "core/column-removal",
    "columnName": "Violent \ncrime \nrate",
    "description": "Remove column Violent \ncrime \nrate"
  },
  {
    "op": "core/column-removal",
    "columnName": "Murder and \nnonnegligent \nmanslaughter \nrate",
    "description": "Remove column Murder and \nnonnegligent \nmanslaughter \nrate"
  },
  {
    "op": "core/column-removal",
    "columnName": "Rape\n(legacy \ndefinition) \nrate4",
    "description": "Remove column Rape\n(legacy \ndefinition) \nrate4"
  },
  {
    "op": "core/column-removal",
    "columnName": "Robbery \nrate",
    "description": "Remove column Robbery \nrate"
  },
  {
    "op": "core/column-removal",
    "columnName": "Aggravated \nassault rate",
    "description": "Remove column Aggravated \nassault rate"
  },
  {
    "op": "core/column-removal",
    "columnName": "Property \ncrime \nrate",
    "description": "Remove column Property \ncrime \nrate"
  },
  {
    "op": "core/column-removal",
    "columnName": "Burglary \nrate",
    "description": "Remove column Burglary \nrate"
  },
  {
    "op": "core/column-removal",
    "columnName": "Motor \nvehicle \ntheft \nrate",
    "description": "Remove column Motor \nvehicle \ntheft \nrate"
  },
  {
    "op": "core/column-removal",
    "columnName": "Larceny-\ntheft rate",
    "description": "Remove column Larceny-\ntheft rate"
  },
  {
    "op": "core/column-rename",
    "oldColumnName": "Violent\ncrime2",
    "newColumnName": "Crimes violents",
    "description": "Rename column Violent\ncrime2 to Crimes violents"
  },
  {
    "op": "core/row-removal",
    "engineConfig": {
      "facets": [
        {
          "type": "list",
          "name": "Lignes étoilées",
          "expression": "row.starred",
          "columnName": "",
          "invert": false,
          "omitBlank": false,
          "omitError": false,
          "selection": [
            {
              "v": {
                "v": true,
                "l": "true"
              }
            }
          ],
          "selectBlank": false,
          "selectError": false
        }
      ],
      "mode": "row-based"
    },
    "description": "Remove rows"
  },
  {
    "op": "core/column-rename",
    "oldColumnName": "Year",
    "newColumnName": "Années",
    "description": "Rename column Year to Années"
  },
  {
    "op": "core/column-rename",
    "oldColumnName": "Murder and\nnonnegligent \nmanslaughter",
    "newColumnName": "Meurtres et homicides involontaires ",
    "description": "Rename column Murder and\nnonnegligent \nmanslaughter to Meurtres et homicides involontaires "
  },
  {
    "op": "core/column-rename",
    "oldColumnName": "Rape\n(legacy \ndefinition)4",
    "newColumnName": "Viols",
    "description": "Rename column Rape\n(legacy \ndefinition)4 to Viols"
  },
  {
    "op": "core/column-rename",
    "oldColumnName": "Robbery",
    "newColumnName": "Vols",
    "description": "Rename column Robbery to Vols"
  },
  {
    "op": "core/column-rename",
    "oldColumnName": "Aggravated \nassault",
    "newColumnName": "Aggressions aggravées",
    "description": "Rename column Aggravated \nassault to Aggressions aggravées"
  },
  {
    "op": "core/column-rename",
    "oldColumnName": "Property \ncrime",
    "newColumnName": "Crimes contre des biens ",
    "description": "Rename column Property \ncrime to Crimes contre des biens "
  },
  {
    "op": "core/column-rename",
    "oldColumnName": "Burglary",
    "newColumnName": "Cambriolages",
    "description": "Rename column Burglary to Cambriolages"
  },
  {
    "op": "core/column-rename",
    "oldColumnName": "Larceny-\ntheft",
    "newColumnName": "Larcins-vols",
    "description": "Rename column Larceny-\ntheft to Larcins-vols"
  },
  {
    "op": "core/column-rename",
    "oldColumnName": "Motor \nvehicle \ntheft",
    "newColumnName": "Vols de véhicules à moteur",
    "description": "Rename column Motor \nvehicle \ntheft to Vols de véhicules à moteur"
  }
]
  

