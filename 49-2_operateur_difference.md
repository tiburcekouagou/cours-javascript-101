## Comparaison avec l'opérateur de différence (`!=` et `!==`)

JavaScript offre également des opérateurs pour vérifier l'inégalité entre deux valeurs :

* `!=` : Inégalité abstraite, qui effectue une conversion de type si nécessaire.
* `!==` : Inégalité stricte, qui ne compare que les valeurs de même type.

Exemples

```js
console.log(5 != '5'); // Affiche false car '5' est converti en 5 avant comparaison
console.log(5 !== '5'); // Affiche true car les types (number et string) sont différents
console.log(null != undefined); // Affiche false car null et undefined sont considérés comme égaux
console.log(null !== undefined); // Affiche true car les types (null et undefined) sont différents
```