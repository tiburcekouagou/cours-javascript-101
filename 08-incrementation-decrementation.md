## Incrémentation et décrémentation
l'incrémentation et la décrémentation sont des opérations courantes pour augmenter ou diminuer la valeur d'une variable de 1. Voici comment elles fonctionnent :  
* **Incrémentation (++)** : L'opérateur d'incrémentation (++) ajoute 1 à la valeur d'une variable.  
````js
let x = 5;
x++; // Équivaut à x = x + 1;
console.log(x); // Affiche 6
```` 
L'opérateur d'incrémentation peut être placé avant (++x) ou après (x++) la variable. Lorsqu'il est placé avant la variable, la valeur est augmentée avant toute autre utilisation de la variable. Lorsqu'il est placé après, la valeur est augmentée après son utilisation. Par exemple :  
````js
let a = 5;
let b = ++a; // a est d'abord incrémenté, puis b prend la valeur de a (a=6, b=6)
console.log(a); // Affiche 6
console.log(b); // Affiche 6

let c = 5;
let d = c++; // c est d'abord affecté à d, puis c est incrémenté (d=5, c=6)
console.log(c); // Affiche 6
console.log(d); // Affiche 5
````  
* **Décrémentation (--)** : L'opérateur de décrémentation (--) soustrait 1 à la valeur d'une variable.  
````js
let y = 10;
y--; // Équivaut à y = y - 1;
console.log(y); // Affiche 9
````
Comme pour l'incrémentation, l'opérateur de décrémentation peut être placé avant (--x) ou après (x--) la variable, avec des effets similaires sur le moment où la valeur est modifiée.L'incrémentation et la décrémentation sont utiles dans les boucles et d'autres situations où vous devez modifier la valeur d'une variable de manière itérative.
