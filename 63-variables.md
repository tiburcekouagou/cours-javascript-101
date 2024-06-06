# 63 - Variables
Une autre utilisation de la `notation entre crochets` sur les objets consiste à accéder à une propriété qui est stockée comme valeur d'une variable. Cela peut être très utile pour parcourir les propriétés d'un objet ou pour accéder à une table de recherche.

## Exemple 1:
Voici un exemple d'utilisation d'une variable pour accéder à une propriété :

```js
    const dogs = {
        Fido: "Mutt",
        Hunter: "Doberman",
        Snoopie: "Beagle"
    };

    const myDog = "Hunter";
    const myBreed = dogs[myDog];
    console.log(myBreed);
```
La chaîne `Doberman` sera affichée dans la console.
    
**NB:** Notez que nous n'utilisons pas de guillemets autour du nom de la variable lorsque nous l'utilisons pour accéder à la propriété car nous utilisons la valeur de la variable, pas le nom .

## Exemple 2:
Définissons une variable  `playerNumber` avec la valeur `16` . Ensuite, utilisons la variable pour rechercher le nom du joueur que nous allons attribuer à une variable `player`.

```js
    const testObj = {
        12: "Namath",
        16: "Montana",
        19: "Unitas"
    };

    const playerNumber = 16;  
    const player = testObj[playerNumber];
```
La valeur de `player` doit être la chaîne `Montana`.
