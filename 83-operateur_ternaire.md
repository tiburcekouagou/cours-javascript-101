# Opérateur ternaire

Les `opérateurs ternaires` sont une manière concise d'écrire des instructions conditionnelles en JavaScript. Ils permettent d'évaluer une condition et de retourner une valeur en fonction de cette condition, le tout en une seule ligne de code. L'opérateur ternaire utilise le symbole `?` pour séparer la condition de l'expression à exécuter si la condition est `vraie`, et le symbole `:` pour séparer l'expression à exécuter si la condition est `fausse`.

## Syntaxe : 

```js
    condition ? expressionSiVrai : expressionSiFaux;
```

## Exemples : 

```js

    //Exemple 1
    let age = 18;
    let message = age >= 18 ? "Vous êtes majeur" : "Vous êtes mineur";
    console.log(message); // Affiche : Vous êtes majeur

    //Exemple 2
    let nombre = 10;
    let parite = nombre % 2 === 0 ? "pair" : "impair";
    console.log(`Le nombre ${nombre} est ${parite}.`); // Affiche : Le nombre 10 est pair.


```