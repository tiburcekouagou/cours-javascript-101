## Fonctions déclaratives
Les fonctions declaratives offrent une syntaxe claire et flexible pour la définition des fonctions .Elles sont particulièrement utiles pour la récursivité,bénéficient du hoisting et améliorent la lisibilité du code.  
```js
const bicycle = {
    gear:2,
    // setGear:function ( newGear){au debut
    setGear ( newGear){//devient 
        "use strict";
        this.gear = newGear;
    }
};
bicycle.setGear(3);
console.log(bicycle.gear);
```