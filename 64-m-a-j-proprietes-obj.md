# 64 - Maj les propriétés dun objet
Après avoir créé un objet JavaScript, vous pouvez mettre à jour ses propriétés à tout moment, comme vous le feriez pour nimporte quelle autre variable. Vous pouvez utiliser la notation par points ou par crochets pour mettre à jour.

## Exemple 1:
Par exemple, regardons l'objet `ourDog` qui représente un chien. Puisque c'est un chien particulièrement heureux, changeons son nom en chaîne `"Happy Camper"`. Voici comment mettre à jour la propriété name de son objet : 

```js
    const ourDog = {
        "name": "Camper",
        "legs": 4,
        "tails": 1,
        "friends": ["everything!"]
    };

    ourDog.name = "Happy Camper";   // ou ourDog["name"] = "Happy Camper";
```

Maintenant, lorsque nous évaluerons `ourDog.name`, au lieu d'obtenir `Camper`, nous obtiendrons son nouveau nom, `"Happy Camper"`.

## Exemple 2:
Mettons à jour la propriété de nom de l'objet `myDog`. Changeons son nom de `Coder` à `"Happy Coder"`. Vous pouvez utiliser la notation par points ou par crochets.

```js
    const myDog = {
        "name": "Coder",
        "legs": 4,
        "tails": 1,
        "friends": ["freeCodeCamp Campers"]
    };
        
    myDog.name = "Happy Coder";   // ou myDog["name"] = "Happy Coder";
```
Vous devez mettre à jour la propriété `name` de `myDog` pour qu'elle soit égale à la chaîne `"Happy Coder"`.

Vous ne devez pas modifier l'objet complet `myDog` définit plut haut
