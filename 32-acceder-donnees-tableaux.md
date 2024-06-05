## Accéder aux données d'un tableau imbriqué
Considérant un tableau 2D, pour trouver un élément spécifique, vous devez d'abord choisir le bon sous-tableau, puis l'élément à l'intérieur de ce sous-tableau.

```js
let matrice = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];

// Accéder aux éléments
console.log(matrice[0][0]); // Affiche 1
console.log(matrice[1][2]); // Affiche 6
console.log(matrice[2][1]); // Affiche 8
```

// Modifier un élément

Avant => `console.log(matrice[0][1]);` // Affiche 2

```js
matrice[0][1] = 10;
```

Après => `console.log(matrice[0][1]);` // Affiche 10
