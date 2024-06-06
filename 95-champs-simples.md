## Champs simples 
Un objet littéral en JavaScript est une manière de créer un objet directement en utilisant la notation littérale, c'est-à-dire en définissant ses propriétés à l'intérieur d'accolades {}. C'est l'une des manières les plus simples et courantes de créer des objets en JavaScript.
```js
// const createPerson =(name, age,genre)=>{
//     return {
//         name: name,
//         age: age,
//         gender:gender
//     }; 

// }

const createPerson = (name, age,genre)=> ({name,age,genre})
console.log(createPerson("Zodiac Hasbros",56,"male"));

// sortie: {name: 'Zodiac Hasbros', age: 56, genre: 'male'}
```
La syntaxe de la fonction fléchée est plus concise que la syntaxe classique des fonctions. Ici, `createPerson` est une fonction fléchée qui prend trois paramètres : `name`, `age`, et `genre`.  
* Les parenthèses autour des accolades `(({ ... }))` indiquent que la fonction retourne un objet littéral.  
* Les accolades seules `({ ... })` seraient interprétées comme le corps d'une fonction si elles n'étaient pas entourées de parenthèses.
* L'objet retourné a trois propriétés : `name`, `age`, et `genre`, dont les valeurs sont respectivement les paramètres `name`, `age`, et `genre` de la fonction.  
L'objet retourné par l'appel de la fonction est le suivant :
```js
{
    name: "Zodiac Hasbros",
    age: 56,
    genre: "male"
}

```
