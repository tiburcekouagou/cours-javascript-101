# 71 - Tableaux imbriqués
Comme nous l'avons vu dans les exemples précédents, les objets peuvent contenir à la fois des objets imbriqués et des tableaux imbriqués. Semblable à l'accès aux objets imbriqués, la notation entre crochets de tableau peut être chaînée pour accéder aux tableaux imbriqués.

## Exemple 1:
Voici un exemple de comment accéder à un tableau imbriqué :

```js 
        const ourPets = [
    {
        animalType: "cat",
        names: [
            "Meowzer",
            "Fluffy",
            "Kit-Cat"
        ]
    },
    {
        animalType: "dog",
        names: [
            "Spot",
            "Bowser",
            "Frankie"
        ]
    }
    ];

    ourPets[0].names[1];
    ourPets[1].names[0];
```

`ourPets[0].names[1]` serait la chaîne `Fluffy`, et o`urPets[1].names[0]` serait la chaîne `Spot`

## Exercice
En utilisant la notation par points et crochets, définissez la variable `secondTree` sur le deuxième élément du tableau `list` à partir du deuxième objet du tableau `myPlants`.

```js
        const myPlants = [
        {
            type: "flowers",
            list: [
            "rose",
            "tulip",
            "dandelion"
            ]
        },
        {
            type: "trees",
            list: [
            "fir",
            "pine",
            "birch"
            ]
        }
        ];

        const secondTree = "";
```
`secondTree` devrait être égal à la chaîne `pine`.
Votre code doit utiliser la notation par points et crochets pour accéder aux propriétés de l'objet `myPlants`.


## SOLUTION

```js
const myPlants = [
    {
        type: "flowers",
        list: [
            "rose",
            "tulip",
            "dandelion"
        ]
    },
    {
        type: "trees",
        list: [
            "fir",
            "pine",
            "birch"
        ]
    }
];

const secondTree = myPlants[1].list[1];
```