# 73 - while loops
Vous pouvez exécuter le même code plusieurs fois en utilisant une `boucle`.

Le premier type de boucle que nous allons apprendre est appelé `boucle while` car elle s'exécute lorsqu’une condition spécifiée est vraie et s'arrête une fois que cette condition n’est plus vraie.

## Exemple 1:
Soit: 

```js
        const ourArray = [];
        let i = 0;

        while (i < 5) {
        ourArray.push(i);
        i++;
        }
```
Dans lexemple de code ci-dessus, la boucle while s'exécutera `5 fois` et ajoutera les nombres `0` à `4` au tableau `ourArray`.

## Exercice:
Essayons de faire fonctionner une boucle while en poussant les valeurs vers un tableau.
Ajoutez les nombres de `5` à `0` (inclus) par ordre décroissant dans `myArray` utilisant une boucle while.

Soit: 

```js
        const myArray = [];
         // ...
```
Vous devriez utiliser une boucle while pour cela.
myArray devrait être égal à [5, 4, 3, 2, 1, 0].

## SOLUTION

```js
        const myArray = [];
        let i = 5;

        while (i >= 0) {
        myArray.push(i);
        i--;
        }
```