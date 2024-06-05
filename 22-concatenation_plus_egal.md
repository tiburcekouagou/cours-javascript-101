## 😎😎Rappelez-vous de l'opérateur +=.
L'opérateur `+=` est utile pour construire des chaînes de caractères de manière incrémentale, surtout lorsque vous devez ajouter plusieurs segments de texte à une chaîne existante dans une boucle ou une séquence d'opérations.

## Avec les variables
L'opérateur `+=` permet de mettre à jour une chaîne de caractères existante en y ajoutant des variables de manière simple et concise. Cette méthode est particulièrement utile lorsqu'il s'agit d'ajouter des segments de texte de manière incrémentale, par exemple dans une boucle ou une séquence d'opérations.

## Exemple 1:
Essayez d'exécuter le code suivant dans votre console JavaScript :
````js
let salutation = "Bonjour";
let nom = "Alice";
salutation += ", "; //a la valeur existant de la variable salutation, on ajoute une virgule, donc désormais la variable salutation contient "Bonjour,"
salutation += nom; //a la valeur existant de la variable salutation, on ajoute la variable nom qui contient la valeur Alice, donc on ajoute le string "Alice" au string "Bonjour," ce qui donne "Bonjour, Alice"
salutation += "!"; //ensuite on ajout un point d'exclamation
console.log(salutation); essayez !!!
````
💡💡L'opérateur `+=` ajoute du contenu à la valeur déjà existante.

## Exemple 2:
````js
let produit = "ordinateur";
let prix = 1200;
let description = "Le prix du ";
description += produit;
description += " est de ";
description += prix;
description += " euros.";
console.log(description);
````
`console.log(description);`  alors ça donne quoi ?