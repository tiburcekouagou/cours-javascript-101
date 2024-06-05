## Utilisation de la "Bracket Notation" sur les Chaînes de Caractères en JavaScript

La `"bracket notation"` est une méthode qui permet d'accéder à des caractères individuels dans une chaîne de caractères en JavaScript. Cette technique est utile pour manipuler et examiner des chaînes de caractères au niveau des caractères individuels.

## Utilisation de la "Bracket Notation"
La `"bracket notation"` utilise des crochets ([]) avec un index pour accéder à un caractère spécifique dans une chaîne. L'index commence à `0`, ce qui signifie que le premier caractère a un index de `0`, le deuxième caractère un index de `1`, et ainsi de suite.

Voici la syntaxe de base :
```js
let chaine = "Bonjour";
let premierCaractere = chaine[0]; // premierCaractere devient "B"
```
💡💡On a vu comment avoir la longueur d'une chaîne de caractère, maintenant on veux acceder chaque caractère de notre chaîne.
Notez que chaque caractère est à une position (index) spécifique.
Prenons le cas de :
```js
    let chaine = "Bonjour";
    console.log(chaine.length) => affichage 7
    index de B => 0
    index de o => 1
    index de n => 2
    index de j => 3
    index de o => 4
    index de u => 5
    index de r => 6
```
Essayez  🚀🚀🚀
```js
    console.log(chaine[0])
    console.log(chaine[1])
    console.log(chaine[2])
    console.log(chaine[3])
    console.log(chaine[4])
    console.log(chaine[5])
    console.log(chaine[6])
```

## Exemple 1: Accéder à des caractères individuels
Essayez d'exécuter le code suivant dans votre console JavaScript :
```js
let mot = "JavaScript";
let premierCaractere = mot[0];
let dernierCaractere = mot[mot.length - 1];
console.log("Le premier caractère est : " + premierCaractere);
console.log("Le dernier caractère est : " + dernierCaractere);
```js