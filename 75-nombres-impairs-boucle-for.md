# 75 - Nombres impairs avec une boucle for
Les boucles `For` n'ont pas besoin d'être itérées une par une. En changeant notre `final-expression`, nous pouvons compter par nombres pairs.
Nous allons commencer à `i = 0` et boucler while `i < 10`. Nous incrémenterons `i` de `2` chaque boucle avec `i += 2`.

## Exemple 1:
Dans l'exemple suivant, nous initialisons avec `i = 0` et itérons pendant que notre condition i < 5 est vraie. Nous incrémenterons i à 1 chaque itération de boucle avec i++ comme expression finale.

```js
    const ourArray = [];

    for (let i = 0; i < 10; i += 2) {
        ourArray.push(i);
    }
```
`ourArray` contiendra désormais `[0, 2, 4, 6, 8]`. Changeons notre initialisation pour pouvoir compter par nombres impairs.

## Exercice:
Poussez les nombres impairs de `1` à `9` dans `myArray` à l’aide d’une `boucle for`.

```js
    const myArray = [];
    // ...
```
Vous devriez utiliser une boucle for pour cela.
`myArray` devrait être égal à `[1, 2, 3, 4, 5]`.

## SOLUTION

```js
    const myArray = [];
        
    for (let i = 1; i <= 9; i += 2) {
        myArray.push(i);
    }
```