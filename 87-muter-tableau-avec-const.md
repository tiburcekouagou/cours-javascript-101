# Muter un Tableau Déclaré avec const en JavaScript

Vous savez déjà qu'une constante ne peut être réassignée.
Alors, c'est pareil, un tableau déclaré avec `const` ne peut pas être réassigné, mais ses éléments internes peuvent être modifiés. 
```js
const monTableau = [3, 5, 7, 9];

monTableau = [1, 2, 4, 6]; // Faire une chose pareille va vous pété une erreur sur la figure, parce que vous êtes en train de réassigner la valeur de la variable monTableau qui est initialisée avec const
```
Mais par contre je peux bien faire ceci:
```js
const monTableau = [3, 5, 7, 9];

monTableau[1] = 9; //ici on modifie la valeur de l'élément à l'index 1 en lui attribuant une nouvelle valeur qui est 9
monTableau[3] = 0; //ici on modifie la valeur de l'élément à l'index 3 en lui attribuant une nouvelle valeur qui est 0

console.log(monTableau) //affiche => [3, 9, 7, 0] (ce qui est différent du tableau initial)
```
Cette capacité à muter le contenu d'un tableau tout en conservant sa référence constante est essentielle pour travailler efficacement avec des structures de données dynamiques.

Les méthodes `push()` pour ajouter des éléments et `pop()` pour supprimer des éléments vous permettent également de modifier un tableau déclaré avec const.