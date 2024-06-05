## Déclaration de variables 
En JavaScript, vous pouvez déclarer des variables en utilisant les mots-clés var, let ou const. Voici comment chaque mot-clé fonctionne :
* **var** : Avant l'introduction de let et const, var était le seul moyen de déclarer des variables en JavaScript. Les variables déclarées avec var sont soit globales, soit locales à la fonction dans laquelle elles sont déclarées. Elles peuvent être redéclarées et réassignées.  
````js
var x = 10;
var y = 20;
x = 30; // Réassignation autorisée
````  
* **let** : let a été introduit dans ECMAScript 6 pour résoudre certains problèmes associés à var. Les variables déclarées avec let sont limitées à la portée du bloc dans lequel elles sont déclarées. Elles ne peuvent pas être redéclarées mais peuvent être réassignées.il est recommandé d'utiliser **let** plutôt que **var** pour déclarer ses variables réassignables  
````js
let a = 10;
let b = 5 
````
