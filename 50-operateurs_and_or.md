# Opérateurs AND / OR

## Opérateur `AND` (`&&`)
L'opérateur `AND` (se lis "and" mais s'écrit `&&`) renvoie `true` si et seulement si les deux opérandes sont `true`. Si l'une des deux conditions est `false`, l'expression entière sera `false`.

Exemple :
```js
    let a = 5;
    let b = 10;
    let c = 15;

    if (a < b && b < c) {
        console.log("Les deux conditions sont vraies.");
    } 
```
Dans cet exemple, `a < b` est `true` et `b < c` est aussi `true`, donc l'expression entière `a < b && b < c` est `true` et "Les deux conditions sont vraies." sera affiché.

## Opérateur `OR` (`||`)
L'opérateur `OR` (se lis "or" mais s'écris `||`) renvoie `true` si au moins l'une des conditions est `true`. Si les deux conditions sont `false`, l'expression entière sera `false`.

Exemple : 
```js
    let x = 5;
    let y = 10;

    if (x > 0 || y < 5) {
        console.log("Au moins une des conditions est vraie.");
    } 
```
Dans cet exemple, `x > 0` est `true`, donc l'expression entière `x > 0 || y < 5` est `true` et "Au moins une des conditions est vraie." sera affiché.


## Utilisation combinée des opérateurs `AND` et `OR`
Vous pouvez combiner les opérateurs `&&` et `||` pour créer des conditions plus complexes.

Exemple combiné : 

```js
    let age = 25;
    let hasPermit = true;

    if ((age >= 18 && age <= 65) || hasPermit) {
        console.log("Vous êtes autorisé à conduire.");
    } 
```
Dans cet exemple, l'expression `age >= 18 && age <= 65` vérifie si l'âge est entre 18 et 65 ans inclus, et l'expression entière `(age >= 18 && age <= 65) || hasPermit` vérifie si l'une des deux conditions est vraie. Si l'une des deux conditions est vraie, le message "Vous êtes autorisé à conduire." sera affiché.