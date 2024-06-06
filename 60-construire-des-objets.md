# 60 - Construire des objets
Vous avez peut-être déjà entendu ce terme `object`.
Les objets sont similaires à `arrays`, sauf qu'au lieu d'utiliser des index pour accéder et modifier leurs données, vous accédez aux données des objets via ce qu'on appelle des `propriétés`.
Les objets sont utiles pour stocker des données de manière structurée et peuvent représenter des objets du monde réel, comme un chient.

## Exemple 1:
Voici un exemple d'objet dog :

```js
    const ourDog = {
    "name": "Camper",
    "legs": 4,
    "tails": 1,
    "friends": ["everithing!"]
    };

```
Dans cet exemple, toutes les propriétés sont stockées sous forme de chaînes, telles que name, legs et tails. Cependant, vous pouvez également utiliser des nombres comme propriétés. 


## Exemple 2:
Vous pouvez même omettre les guillemets pour les propriétés de chaîne d'un seul mot, comme suit :

```js
const anotherObject = {
  make: "Ford",
  5: "five",
  "model": "focus"
};
```
Cependant, si votre objet possède des propriétés autres que des chaînes, JavaScript les transtypera automatiquement sous forme de chaînes.
        
