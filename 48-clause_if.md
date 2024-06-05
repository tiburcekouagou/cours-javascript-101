### Clause if
L'instruction `if` en JavaScript est utilisée pour exécuter un bloc de code **`seulement si`** une condition donnée est vraie.

```js
    if (condition) {
        // Code à exécuter si la condition est vraie
    }
```

Explication
* `if` : Mot-clé utilisé pour introduire une condition.
* `condition` : Expression qui est évaluée. Si elle est vraie (true), le bloc de code à l'intérieur des accolades est exécuté.
* `Bloc de code` : Code qui est exécuté uniquement si la condition est vraie. Ce bloc est délimité par des accolades `{}`.

Exemple : 
```js
    let number = 5;

    if (number > 0) {
        console.log("Le nombre est positif.");
    }
```