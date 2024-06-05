## Assignation avec une valeur retournée

```js
let changed = 0;

function change(num) {
    return (num + 5) / 3;
}

changed = change(10);

let processed = 0;

function processArg(num) {
    return (num + 3) / 5;
}

```

Il est facile d'assigner à une variable ce que retourne une fonction. Ci-dessus nous avons, une fonction `change`. On lui passe un nombre et il retourne le résultat d'une expression mathématique. Quand on appelle la fonction `change` et qu'on lui passe l'argument `10`, la valeur retournée par la fonction sera stockée dans la variable `changed`;

On pourrait faire pareil aussi pour la fonction `processArg`. A vous de jouer

```js
let processed = 0;

function processArg(num) {
    return (num + 3) / 5;
}
// modifier le code ci-dessous
processArg(32); 
```