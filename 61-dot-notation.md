# 61 - Dot notation
Il existe deux manières d'accéder aux propriétés d'un objet : **`la notation par points`** ( .) et **`la notation par crochets`** ([]), similaire à un tableau.   
`La notation par points` est ce que vous utilisez lorsque vous connaissez à l’avance le nom de la propriété à laquelle vous essayez d’accéder.

## Exemple 1:
Voici un exemple d'utilisation de la notation par points ( .) pour lire la propriété d'un objet :

```js
const utilisateur = {
    nom: "Doe",
    prenom: "John"
};

const nomVal = utilisateur.nom;
const prenomVal = utilisateur.prop2;
```
`nomVal` aurait une valeur égale à `Doe` et `prenom` aurait une valeur égale à `John`.

## Exemple 2:
Lisez les valeurs des propriétés liées à `testObj` en utilisant de la `notation par points`. Définissez la variable `hatValue` égale à la propriété de l'objet `hat` et définissez la variable `shirtValue` égale à la propriété de l'objet `shirt`.

```js
const testObj = {
    hat: "ballcap",
    shirt: "jersey",
    shoes: "cleats"
};
        
const hatValue = testObj.hat;      
const shirtValue = testObj.shirt; 
```
`hatValue` aurait une valeur égale à `ballcap` et `shirtValue` aurait une valeur égale à `jersey`.
    