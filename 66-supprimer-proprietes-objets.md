# Supprimer les propriétés d'un objet

Nous pouvons également supprimer les propriétés des objets comme ceci : `delete ourDog.bark`;

## Exemple 1:
Soit: 

```js
    const ourDog = {
        "name": "Camper",
        "legs": 4,
        "tails": 1,
        "friends": ["everything!"],
        "bark": "bow-wow"
    };

    delete ourDog.bark;
```
Après la dernière ligne ci-dessus, `ourDog` cela ressemble à :

```bash
{
    "name": "Camper",
    "legs": 4,
    "tails": 1,
    "friends": ["everything!"]
}
```

## Exemple 2:
Supprimez la propriété `tails` de `myDog`. Vous pouvez utiliser la notation par points ou par crochets.

```js
    const myDog = {
        "name": "Happy Coder",
        "legs": 4,
        "tails": 1,
        "friends": ["freeCodeCamp Campers"],
        "bark": "woof"
    };

    delete myDog.tails;
```

Vous devez supprimer la propriété `tails` de `myDog`.
Vous ne devez pas modifier la configuration de `myDog` et vous devew obtenir:
```
{
    "name": "Happy Coder",
    "legs": 4,
    "friends": ["freeCodeCamp Campers"],
    "bark": "woof"
};
```

