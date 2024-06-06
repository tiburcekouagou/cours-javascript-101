# 78 - Boucles for imbriquées
Si vous disposez d'un tableau multidimensionnel, vous pouvez utiliser la même logique que le point de cheminement précédent pour parcourir à la fois le tableau et tous les sous-réseaux.

## Exemple:
Voici un exemple:

```js
    const arr = [
        [1, 2], [3, 4], [5, 6]
    ];

    for (let i = 0; i < arr.length; i++) {
        for (let j = 0; j < arr[i].length; j++) {
            console.log(arr[i][j]);
        }
    }
```
Cela génère chaque sous-élément `arr` un par un. Notez que pour la boucle interne, nous vérifions la longueur de  `arr[i]`, puisque `arr[i]` est lui-même un tableau.

## Exercice:
Modifiez la fonction multiplyAllpour qu'elle renvoie le produit de tous les nombres des sous-tableaux de arr.

```js
    function multiplyAll(arr) {
        let product = 1;
        // ...
        return product;
    }

    multiplyAll([[1, 2], [3, 4], [5, 6, 7]]);
```
`multiplyAll([[1], [2], [3]])` devrait retourner `6`   
`multiplyAll([[1, 2], [3, 4], [5, 6, 7]])` devrait retourner `5040`   
`multiplyAll([[5, 1], [0.2, 4, 0.5], [3, 9]])` devrait retourner `54`   

## SOLUTION

```js
function multiplyAll(arr) {
    let product = 1;

    for (let i = 0; i < arr.length; i++) {
        for (let j = 0; j < arr[i].length; j++) {
            product *= arr[i][j];
            }
        }
    return product;
}

multiplyAll([[1, 2], [3, 4], [5, 6, 7]]);
```