## push()
La méthode `push()` ajoute un ou plusieurs éléments à la fin d'un tableau. Elle retourne la nouvelle taille du tableau.

```js
let fruits = ["pomme", "banane", "cerise"]; 

let countArray = fruits.push("avocat"); 
// frutis = ["pomme", "banane", "cerise", "avocat"] 
// countArray vaudra 4 (la nouvelle longueur du tableau)

const count = fruits.push("papaye", "ananas", "mandarine"); 
// fruits = ["pomme", "banane", "cerise", "avocat", "papaye", "ananas", "mandarine"]
count vaudra 7 (la nouvelle longueur du tableau)

```