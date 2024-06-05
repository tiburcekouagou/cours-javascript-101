## Accéder aux données d'un tableau simple
Les tableaux sont indexés à partir de `zéro`: le premier élément d'un tableau a pour indice `0`, et la position du dernier élément est donnée par la propriété `.length` (propriété permettant d'avoir la taille d'un tableau) moins `1`.

**NB**: Si on utilise un indice en dehors de cet intervalle, le résultat sera `'undefined'`

```js
let fruits = ["pomme", "banane", "cerise"];
console.log(fruits[0]); // "pomme"
console.log(fruits[1]); // "banane"
console.log(fruits[2]) || console.log(fruits[fruits.length - 1]); // "cerise"

```