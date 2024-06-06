## Littéraux de Gabarit
Les littéraux de gabarit (template literals) en JavaScript sont une fonctionnalité puissante qui permet d'inclure des expressions et des variables dans des chaînes de caractères de manière concise et lisible. Ils utilisent les backticks (accent grave, __`__  au lieu des guillemets simples **__(')__** ou doubles **__(")__**. Voici comment les utiliser :  
### Syntaxe de base  
Les littéraux de gabarit permettent d'insérer des expressions JavaScript à l'intérieur d'une chaîne de caractères en utilisant la syntaxe `${expression}`.
```js
let nom = 'Alice';
let age = 25;
let message = `Bonjour, je m'appelle ${nom} et j'ai ${age} ans.`;
console.log(message); // Affiche "Bonjour, je m'appelle Alice et j'ai 25 ans."
```
### Interpolation de variables et expressions
Vous pouvez inclure des expressions complexes et des appels de fonctions à l'intérieur des littéraux de gabarit.  
```js
let x = 10;
let y = 20;
let resultat = `La somme de ${x} et ${y} est ${x + y}.`;
console.log(resultat); // Affiche "La somme de 10 et 20 est 30."
```
### Multi-lignes  
Les littéraux de gabarit permettent également d'inclure des chaînes de caractères sur plusieurs lignes sans avoir besoin d'opérateurs de concaténation (+) ou de caractères d'échappement (\n).  
```js
let poeme = `Les feuilles tombent,
Les arbres se dénudent,
L'automne est là.`;

console.log(poeme);
// Affiche :
// Les feuilles tombent,
// Les arbres se dénudent,
// L'automne est là.
```  
Les littéraux de gabarit peuvent être associés à des fonctions spéciales appelées "tag functions" qui permettent de manipuler les parties littérales et les expressions interpolées avant de produire la chaîne finale.

```js
const result = {
    success:["max-length","no-amd","prefer-arrow-functions"],
    failure:["no-var","var-on-top","linebreack"],
    skipped: ["id-blacklist","no-dup-keys"]
};
function makeList(arr) {
    const resultDisplayArray = [];
    for(let i = 0; i <arr.length; i++){
        resultDisplayArray.push(`<li class = "text-waning">${arr[i]}</li>`)
    }
    return resultDisplayArray;
}

    const resultDisplayArray = makeList(result.failure);

    console.log(resultDisplayArray);


    // redu
    [
    '<li class="text-warning">no-var</li>',
    '<li class="text-warning">var-on-top</li>',
    '<li class="text-warning">linebreak</li>'
]
```