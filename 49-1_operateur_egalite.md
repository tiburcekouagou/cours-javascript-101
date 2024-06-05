## Opérateur d'égalité
L'opérateur d'égalité en JavaScript est utilisé pour comparer deux valeurs et déterminer si elles sont égales.
JavaScript offre deux types d'opérateurs d'égalité : 

###  Opérateur d'égalité abstraite (`==`)
L'opérateur `==` compare deux valeurs pour vérifier si elles sont égales après conversion de type. Cela signifie que si les valeurs comparées sont de types différents, JavaScript tente de les convertir à un type commun avant de les comparer.

Exemple d'utilisation : 
```js
console.log(5 == '5'); // Affiche true car '5' est converti en 5 avant comparaison
console.log(true == 1); // Affiche true car true est converti en 1 avant comparaison
console.log(false == 0); // Affiche true car false est converti en 0 avant comparaison
```

### Opérateur d'égalité stricte (`===`)
L'opérateur `===` compare deux valeurs pour vérifier si elles sont exactement égales, c'est-à-dire à la fois en termes de valeur et de type. Aucune conversion de type n'est effectuée.

Exemple d'utilisation : 

```js
console.log(5 === '5'); // Affiche false car les types (number et string) sont différents
console.log(true === 1); // Affiche false car les types (boolean et number) sont différents
console.log(false === 0); // Affiche false car les types (boolean et number) sont différents
console.log(5 === 5); // Affiche true car les valeurs et les types sont identiques
```
