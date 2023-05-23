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
