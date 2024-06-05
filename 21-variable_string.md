## Construction de Chaînes de Caractères avec des Variables en JavaScript

La construction de chaînes de caractères avec des variables est une pratique courante en JavaScript. Elle permet de créer des messages dynamiques et de manipuler les données textuelles de manière flexible. Vous pouvez facilement remplacer les valeurs des variables pour générer de nouvelles chaînes de caractères sans modifier l'ensemble de votre code.

## Exemple 1:
````js
const variable1 = "Alice";
const variable2 = "Bonjour, " + variable1 + "!";
console.log(variable2); //Bonjour, Alice!
````
💡💡 Alors ici, la chaîne de caractère contenue dans la variable2 est créée en combinant la variable1.

## Exemple 2 : Créer une Phrase avec des Variables
Utilisez des variables et des expressions arithmétiques pour construire une phrase :
````js
const nom = "Charlie";
const age = 30;
const anneeDeNaissance = 2024 - age;
const info = nom + " a " + age + " ans et est en " + anneeDeNaissance + ".";
console.log(info);
````
Essayez ce code !🎲

Continuez à explorer ces concepts en créant vos propres exemples et en expérimentant avec différentes méthodes pour construire des chaînes de caractères avec des variables. Go Go Go !💪💪
