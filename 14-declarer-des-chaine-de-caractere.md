
## Déclarer des chaînes de caractère
vous pouvez déclarer des chaînes de caractères en les entourant de guillemets simples (') ou doubles ("). Voici quelques exemples :
````js
let nom = 'Alice'; // Utilisation de guillemets simples
let message = "Bonjour, monde !"; // Utilisation de guillemets doubles
````  
Vous pouvez également utiliser des backticks (accent grave, `) pour déclarer des chaînes de caractères appelées "templates de chaînes de caractères" (string templates) qui permettent l'insertion de variables et l'évaluation d'expressions à l'intérieur de la chaîne en utilisant ${}. Par exemple :  
````js
let x = 10;
let y = 20;
let resultat = `La somme de ${x} et ${y} est ${x + y}.`; // Utilisation des templates de chaînes de caractères
console.log(resultat); // Affiche "La somme de 10 et 20 est 30."
````  