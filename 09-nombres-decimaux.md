
## Nombres Décimaux
les nombres décimaux, également appelés nombres à virgule flottante, sont des nombres qui peuvent avoir une partie fractionnaire. Par exemple, 3.14 est un nombre décimal. Voici quelques points importants à connaître sur les nombres décimaux en JavaScript :  
* **Déclaration**: Vous pouvez déclarer des nombres décimaux en les écrivant avec un point décimal.  
````js
let pi = 3.14;
````
* **Opérations mathématiques** : Vous pouvez effectuer des opérations mathématiques sur les nombres décimaux, comme l'addition, la soustraction, la multiplication et la division.  
````js
let x = 10.5;
let y = 2.5;
let sum = x + y; // Addition
let difference = x - y; // Soustraction
let product = x * y; // Multiplication
let quotient = x / y; // Division
````
* **Précision** : Les nombres décimaux en JavaScript ont une précision limitée en raison de la façon dont ils sont représentés en interne. Cela peut parfois entraîner des erreurs d'arrondi dans les calculs.  
````js
console.log(0.1 + 0.2); // Affiche 0.30000000000000004 (et non 0.3)
````  
* **Conversion** : Vous pouvez convertir des nombres décimaux en entiers en utilisant les fonctions `parseInt()`.  
````js
let floatNum = 10.5;
let num = parseInt(floatNum); // Convertit le nombre décimal 10.5 en un nombre entier
````  

 Vous pouvez faire de même un conversion d'un nombre entiers en un nombre décimal en utilisant les fonctions `parseFloat()`.

````js
let num = 10;
let floatNum = parseFloat(num); // Convertit le nombre entier 10 en un nombre décimal 10.0
// NB: La console pourrait afficher juste 10 après conversion. Mais logiquement,
// la variable "floatNum" est considérée comme un nombre décimal
````  