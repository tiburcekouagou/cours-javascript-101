## L'Immutabilité des Chaînes de Caractères en JavaScript

En JavaScript, les chaînes de caractères (ou strings) sont `immuables`, ce qui signifie qu'une fois qu'une chaîne de caractères est créée, elle ne peut pas être modifiée.
L'immuabilité garantit que les chaînes de caractères ne peuvent pas être modifiées après leur création, ce qui rend le code plus sûr et prévisible. Cela ne veux par dire que la chaine de caractère ne peux pas être changée. Mais les caractères individuellement ne peuvent pas être modifiés.

Supposons que j'ai :
```js
let monString = "Hello world";
console.log(monString[0]) //affiche H
//Mais si vous essayez de changer la valeur de H en F par exemple en faisant:
monString[0] = "F"; //et ensuite vous essayez d'afficher la variable monString
console.log(monString) //vous affiche toujours "Hello world" mais pas "Fello world" 😎😎
```
Evidemmment vous pouvez bien changer tout le "Hello world" en autre chaîne de caractère.