## Exercice Stand in line

```js
function nextInLine(arr, item) {
    // 
    return item;
}

let testArray = [1, 2, 3, 4, 5];

console.log("Avant: " + JSON.stringify(testArray));
console.log(nextInLine(testArray, 6));
console.log("Après: " + JSON.stringify(testArray));
```

## Les `queue`
Une `queue` en programmation est un peu comme une file d'attente dans la vraie vie. Imagine que tu attends pour monter dans un bus. Les gens arrivent et se mettent à la fin de la file. La première personne qui arrive est la première à monter dans le bus, et ainsi de suite. En programmation, une queue fonctionne de la même manière : les éléments sont ajoutés à la fin de la file et retirés du début, suivant le principe du "premier arrivé, premier servi". C'est utile pour traiter les tâches dans l'ordre où elles sont arrivées.

## Exercice

Dans cette leçon, nous allons essayer de simuler le mode de fonctionnement des `queue` avec la fonction nextInLine. Cette fonction, prend deux arguments: 
- `arr` qui est un tableau avec des nombres. Ces nombres représentent la file d'attente 
- `item` représente un nombre qu'on veut insérer dans le tableau (donc dans la file d'attente).

La fonction `nextInLine` devrait donc ajouter l'`item` à la fin du tableau, et devrait ensuite le renvoyer.

Exemple: 

```js
console.log("Avant: " + JSON.stringify(testArray)); // renvoie [1, 2, 3, 4, 5]
console.log(nextInLine(testArray, 6)); // renvoie 6
console.log("Après: " + JSON.stringify(testArray)); // renvoie [1, 2, 3, 4, 5, 6]
```

## Bonus

Faite en sorte que la fonction `nextInLine` ajoute l'`item` et retire le premier élément. Et donc, on implémente le principe de: "La première personne qui arrive est la première à monter dans le bus".

```js
function nextInLine(arr, item) {
    // Vous pouvez modifiez le code ci-dessous
    return item;
}

let testArray = [1, 2, 3, 4, 5];

console.log("Avant: " + JSON.stringify(testArray)); // renvoie [1, 2, 3, 4, 5]
console.log(nextInLine(testArray, 6)); // renvoie 6
console.log("Après: " + JSON.stringify(testArray)); // renvoie [2, 3, 4, 5, 6]
```