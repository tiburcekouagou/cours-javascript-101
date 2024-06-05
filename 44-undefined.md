## Comprendre les valeurs  `undefined` retournées par une fonction

```js
// Exemple
let sum = 0;
function addThree() {
    sum = sum + 3;
}
```

Les fonctions peuvent avoir des instructions `return` comme elle peuvent ne pas en avoir. Dans le cas ci-dessus, la fonction `"addThree"` ajoute `3` à la variable `sum` qui est une variable globale vu qu'elle est définie hors de la fonction. Remarquez qu'il n'y a pas d'instruction `return` dans la fonction. Et donc, si nous ne spécifions pas de valeur de retour, la valeur de retour sera `undefined`. Vous pouvez essayer de *console loguer* ce que retourne la fonction `addThree` pour vérifier.

A présent, nous allons créer une fonction similaire.

```js
function addFive() {
    sum += 5; // ou pourrait écrire: sum = sum + 5;
}
```

La fonction `addFive` ajoute également `5` à la variable `sum` mais ne retourne rien.

Question: Quel est le type de retour de la fonction `addFive`

Vous pouvez essayer la commande suivante pour vérifier:

```js
function addFive() {
    sum += 5; // ou pourrait écrire: sum = sum + 5;
}

console.log(addFive()); // on vérifie ce que retourne addFive()
```