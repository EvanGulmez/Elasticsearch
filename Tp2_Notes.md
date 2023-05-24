Multi-match

Utilisation de multi_match pour rechercher sur plusieurs champs avec des poids différents et choisir le type de recherche (best_fields, most_fields, cross_fields, phrase, phrase_prefix).

best_fields : recherche sur le champ qui donne le meilleur résultat.

most_fields : recherche sur le champ qui donne le plus de résultats.

cross_fields : recherche sur les champs en les concaténant.

phrase : recherche sur une phrase.

phrase_prefix : recherche sur une phrase avec un préfixe.

Bool
Utilisation de bool pour effectuer des requêtes booléennes.

must : doit correspondre.

must_not : ne doit pas correspondre.

should : peut correspondre.

filter : doit correspondre, mais n'a pas d'impact sur le score.

Agrégations
Utilisation de aggs pour effectuer des agrégations.

terms : agrégation sur les champs de type keyword.

date_histogram : agrégation sur les champs de type date.

Mapping
Utilisation de mapping pour définir le mapping d'un index (les types).

properties : définition des propriétés d'un type.

type : définition du type d'une propriété.

analyzer : définition de l'analyseur d'une propriété (standard, lowercase, french, ...).

fields : définition de plusieurs champs pour une même propriété (avec des analyseurs différents).

keyword : définition d'une propriété de type keyword.

text : définition d'une propriété de type text.

date : définition d'une propriété de type date avec un format.

format : définition du format d'une propriété de type date.

''''     Explication des données indexées    ''''

- Indexation des données: La première étape consiste à effectuer l'indexation des données dans Elasticsearch, en les ajoutant à un index spécifique, ce qui correspond à une base de données (BDD).

- Requêtes de recherche : Une fois les données indexées, il devient possible d'effectuer des requêtes de recherche afin de récupérer et analyser ces données. Les différents types de requêtes sont détaillés dans le fichier "TP2 notes.md".

- Agrégations: Les agrégations sont une fonctionnalité puissante d'Elasticsearch permettant d'analyser les données indexées. Elles permettent de regrouper, filtrer et calculer des statistiques sur les données. Le fichier "TP2 notes.md" présente les différents types d'agrégations disponibles.

- Analyze (Analyseur de texte): Pour faciliter la recherche de texte dans les données indexées, Elasticsearch dispose d'un analyseur de texte intégré. Cet analyseur divise le texte en termes individuels appelés tokens, les normalise en minuscules, supprime les mots vides et applique d'autres traitements. Ainsi, il prend en compte la correspondance des mots lors de la recherche.

- Relevancy (pertinence) : Lors de la recherche, Elasticsearch utilise un algorithme de pertinence pour classer les résultats en fonction de leur pertinence par rapport à la requête effectuée.

- Visualisations : En combinaison avec Kibana, une plateforme de visualisation de données, Elasticsearch permet de créer des tableaux de bord interactifs, des graphiques et des visualisations basés sur les données indexées.