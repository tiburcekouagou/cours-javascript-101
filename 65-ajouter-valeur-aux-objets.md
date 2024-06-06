# Ajouter de nouvelles propriétés
Vous pouvez ajouter de nouvelles propriétés aux objets JavaScript existants de la même manière que vous les modifieriez.

## Exemple 1:
Voici comment ajouter une propriété bark à ourDog :

```js
    const ourDog = {
        "name": "Camper",
        "legs": 4,
        "tails": 1,
        "friends": ["everything!"]
    };

    ourDog.bark = "bow-wow";  // ou ourDog["bark"] = "bow-wow";
```
Maintenant, quand nous évaluerons `ourDog.bark`, nous aurons son aboiement `bow-wow`.

## Exemple 2:        
Ajoutez une propriété `bark` à `myDog` et définissez-la sur un aboiement de chien, tel que `"woof"`. Vous pouvez utiliser la notation par points ou par crochets.

```js
    const myDog = {
        "name": "Happy Coder",
        "legs": 4,
        "tails": 1,
        "friends": ["freeCodeCamp Campers"]
    };

    myDog.bark = "woof";  // ou myDog["bark"] = "woof";
```
Vous devez ajouter la propriété `bark` à `myDog`.
Vous ne devez pas ajouter d'éléments `bark` à l'initialisation de `myDog`.