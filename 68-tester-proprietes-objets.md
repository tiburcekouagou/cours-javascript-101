# 68 - Tester les propriétés d'un objet

Pour vérifier si une propriété sur un objet donné existe ou non, vous pouvez utiliser la méthode `.hasOwnProperty()`
`someObject.hasOwnProperty(someProperty)` renvoie `true` ou `false` selon que la propriété se trouve ou non sur l'objet.

## Exemple:
Soit : 

```js
    function checkForProperty(object, property) {
    return object.hasOwnProperty(property);
    }

    checkForProperty({ top: 'hat', bottom: 'pants' }, 'top'); // true
    checkForProperty({ top: 'hat', bottom: 'pants' }, 'middle'); // false
```
Le premier appel de la fonction `checkForProperty` renvoie `true`, tandis que le second renvoie `false`.

## Exercice:
Modifiez la fonction `checkObj` pour tester si l'objet passé au paramètre de fonction `obj` contient la propriété spécifique passée au paramètre de fonction `checkProp`.
Si la propriété transmise à `checkProp` est trouvée sur `obj`, renvoie la valeur de cette propriété. Sinon, revenez `Not Found`.
Soit : 

```js
    function checkObj(obj, checkProp) {
    return "Change Me!";
    }
```
`checkObj({gift: "pony", pet: "kitten", bed: "sleigh"}, "gift")` devrait renvoyer la chaîne `pony`.    
`checkObj({gift: "pony", pet: "kitten", bed: "sleigh"}, "pet")` devrait renvoyer la chaîne `kitten`.    
`checkObj({gift: "pony", pet: "kitten", bed: "sleigh"}, "house")` devrait renvoyer la chaîne `Not Found`.   
`checkObj({city: "Seattle"}, "city")` devrait renvoyer la chaîne Seattle.   
`checkObj({city: "Seattle"}, "district")` devrait renvoyer la chaîne `Not Found`.    
`checkObj({pet: "kitten", bed: "sleigh"}, "gift")` devrait renvoyer la chaîne `Not Found`.   


## SOLUTION

```js
function checkObj(obj, checkProp) {
    if (obj.hasOwnProperty(checkProp)){
        return obj[checkProp];
    } else
    return "Not Found";
}
```
