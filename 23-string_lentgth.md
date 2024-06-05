## Trouver la longueur d'une chaîne de caractère

Connaître la longueur d'une chaîne de caractères est une opération courante en JavaScript. La longueur d'une chaîne peut être utile dans de nombreux contextes, tels que la validation des entrées utilisateur, la manipulation de texte ou la génération dynamique de contenu.

## Utilisation de la Propriété `.length`
La propriété `.length` (point length) permet de trouver la longueur d'une chaîne de caractères.
💡💡 La longueur d'une chaîne de caractère n'est rien d'autre que le nombre de caractère contenu dans la chaîne.
Voici la syntaxe de base :

## Exemple 1:
````js
let chaine = "Hello";
let longueur = chaine.length; // longueur égale 5
````
💡💡 Ici le string `"Hello"` est stocké dans la variable `chaine`.
Pour trouver la longueur de `"Hello"`, on va donc prendre la variable `chaine` à qui on ajoute `.length` (length veut dire longueur).
D'où : `let longueur = chaine.length nous donne 5;`

## Exemple 2:
Essayez d'exécuter le code suivant dans votre console JavaScript :
````js
let message = "Bonjour tout le monde";
let longueur = message.length;
console.log("La longueur du message est : " + longueur);
````
💡💡 Notez qu'en programmation, les espaces sont également des caractères !

## Exemple 3:
Déclarez une variable contenant une chaîne et trouvez sa longueur :
````js
let nom = "Alice";
let longueurNom = nom.length;
console.log("Le nom " + nom + " a " + longueurNom + " caractères.");
````
## Exemple 4:
Utilisez la longueur d'une chaîne pour afficher un message différent selon sa longueur :
````js
let password = "123456";
if (password.length < 8) {
  console.log("Le mot de passe est trop court.");
} else {
  console.log("Le mot de passe a une longueur adéquate.");
}
````

Continuez à explorer ces concepts en créant vos propres exemples et en expérimentant avec la propriété .length dans différents contextes. Go Go Go !💪💪🔥🔥