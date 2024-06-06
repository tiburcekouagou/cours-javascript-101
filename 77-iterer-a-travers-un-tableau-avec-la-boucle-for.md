# 77 - Itérer à travers un tableau avec la boucle for
Une tâche courante en JavaScript consiste à parcourir le contenu d’un tableau. Une façon de procéder consiste à utiliser une boucle for. 

## Exemple 1:
Ce code affichera chaque élément du tableau arr sur la console :

```js
        const arr = [10, 9, 8, 7, 6];

        for (let i = 0; i < arr.length; i++) {
        console.log(arr[i]);
        }
```
N'oubliez pas que les tableaux ont une indexation de base zéro, ce qui signifie que le dernier index du tableau est length - 1. Notre condition pour cette boucle est i < arr.length, qui arrête la boucle lorsque i est égale à length. Dans ce cas, la dernière itération est i === 4 c'est-à-dire quand i devient égale arr.length - 1 et sort 6 vers la console. Puis i augmente jusqu'à 5, et la boucle se termine car i < arr.length est false.

## Exercice:
Déclarez et initialisez une variable total egale 0. Utilisez une boucle for pour ajouter la valeur de chaque élément du tableau myArr à total.

```js
    const myArr = [2, 3, 4, 5, 6];
    // ...
```
`total` doit être déclaré et initialisé à `0`.   
`total` devrait être égal à `20`.   
Vous devez utiliser une boucle for pour parcourir `myArr`.   
Vous ne devez pas tenter d'attribuer directement la valeur `20` à `total`.

## SOLUTION

```js
    const myArr = [2, 3, 4, 5, 6];
    let total = 0;

    for (let i = 0; i < myArr.length; i++) {
            total += myArr[i]
    }
```