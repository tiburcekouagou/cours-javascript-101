# 62 - Bracket notation

La deuxième façon d'accéder aux propriétés d'un objet est la `notation entre crochets` ( []). Si la propriété de l'objet auquel vous essayez d'accéder comporte un espace dans son nom, vous devrez utiliser la `notation entre crochets`.   
Cependant, vous pouvez toujours utiliser la `notation entre crochets` sur les propriétés d'objet sans espaces.

## Exemple 1:
Voici un exemple d'utilisation de la `notation entre crochets` pour lire la propriété d'un objet :

```js
    const user = {
        "Nom Utilisateur": "Kirk",
        "Prenom Utilisateur": "Spock",
        "profression": "Développeur JavaScript"
    };

    user["Nom Utilisateur"];
    user['Prenom Utilisateur'];
    user["profression"];
```

`user["Nom Utilisateur"]` serait la chaîne `Kirk`, `user['Prenom Utilisateur']` serait la chaîne Spock et `user["profression"]` serait la chaîne `Développeur JavaScript`.
        
**NB:** Notez que les noms de propriétés contenant des espaces **doivent être entre guillemets (simples ou doubles)**.

## Exemple 2:
Lisons les valeurs des propriétés `"an entree"` et `"the drink"` de `testObj` en utilisant de la notation entre crochets et attribuez-les respectivement à `entreeValue` et `drinkValue`.

```js
    const testObj = {
    "an entree": "hamburger",
    "my side": "veggies",
    "the drink": "water"
    };

    const entreeValue = testObj["an entree"];   
    const drinkValue = testObj["the drink"];    
```

La valeur de `entreeValue` est égale à `hamburger`   
La valeur de `drinkValue` est égale à `water`   
