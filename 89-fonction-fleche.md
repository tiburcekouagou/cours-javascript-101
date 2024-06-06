# Fonctions Fléchées en JavaScript

Voici une fonction classique comme vous le connaîssez:
```js
function maFunction() {
    //Instruction à exécuter par ma function
    console.log('Je suis une déclaration de fonction');
}
maFunction();
```

Une autre fonction
```js
//Ceci est une fonction anonyme, remarquez que la syntaxe est un peu particulière
const anonyme = function() {
    
    return new Date();
}
//La fonction anonyme n'a pas de nom et est stockée dans une variable
```
Javascript nous offre une autre façon pour définir une fonction, il s'agit des **`fonctions fléchées`**.
Les `fonctions fléchées` (`arrow functions`) en JavaScript, introduites dans ECMAScript 6 (ES6), offrent une syntaxe concise pour écrire des fonctions. Elles ont des comportements différents par rapport aux fonctions traditionnelles, notamment en ce qui concerne la gestion du mot-clé this (on ne va pas s'occuper du mot clé this ici).

On peux transformer une fonction anonyme en une fonction fléchée très rapidement 😉
Reprenons notre fonction anonyme plus haut.
On va retirer le mot-clé fonction et mettre une flèche après les parenthèses, comme ceci:
```js
const anonyme = () => {
    return new Date();
}
```
On peut encore aller plus loin.
Notre fonction retourne une seule valeur, du coup, on peut supprimer le mot-clé ruturn et les accolades, et on aura donc:
```js
const anonyme = () => new Date();
```
ça c'est la version finale de notre fonction fléchée, simple et courte!

Alors tout comme une fonction normale, vous pouvez passer des paramètre à votre fonction fléchée.
```js
const myConcat = (arr1, arr2) => arr1.concat(arr2)
console.log(myConcat([4, 6], [2, "O"])); //affiche [ 4, 6, 2, "O" ]
```
Dans cet exemple, notre fonction retourne la concatenation de deux tableaux. Elle prend en paramètres deux tableaux.


## Exercice 1 : Calculer le Carré d'un Nombre
Objectif : Créez une fonction fléchée qui prend un nombre en paramètre et retourne son carré.

## Exercice 2 : Vérifier si un Nombre est Pair
Objectif : Créez une fonction fléchée qui prend un nombre en paramètre et retourne true s'il est pair, false sinon.