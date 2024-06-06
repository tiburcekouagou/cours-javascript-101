
## Déstructuration
La déstructuration d'objets est une fonctionnalité qui permet d'extraire des valeurs de propriétés d'un objet et de les assigner à des variables individuelles  
#### Exemple 1 
```js
let voxel = {
    x:3.6,
    y:7.4,
    z:6.54
}
let x = voxel.x ;// x = 3.6
let y = voxel.y ;// y = 7.4
let z = voxel.z ;// z = 6.54

const { x: a, y:b, z:c } = voxel // a = 3.6  ,b = 7.4, c = 6.54
```  
`{ x: a, y: b, z: c }` : Cela indique que vous extrayez les valeurs des propriétés `x`, `y` et `z` de l'objet voxel et les assignez respectivement aux variables a, b et c. La syntaxe `{ propriété: variable }` signifie que la valeur de la propriété est assignée à la variable avec le nom spécifié.  
#### Exemple 2
```js
const AVG_TEMPERATURES = {
    today : 77.5,
    tomorrow : 79
};
function getTempOfTomorrow(avgTemperatures) {
    "use strict";
    const { tomorrow : tempOfTomorrow } = avgTemperatures
    return tempOfTomorrow
}
console.log (getTempOfTomorrow(AVG_TEMPERATURES));
```  
Que retourne ce code ❓  

### La déstructuration avec des objets imbriqués
La déstructuration avec des objets imbriqués (nested objects) permet d'extraire facilement des valeurs des niveaux inférieurs de l'objet. Voici comment procéder :  
#### Exemple de base avec objets imbriqués  
Imaginons un objet représentant une personne avec des détails d'adresse imbriqués :  
```js
let personne = {
    nom: 'Alice',
    age: 25,
    adresse: {
        rue: '123 Rue de Paris',
        ville: 'Paris',
        codePostal: '75001'
    }
};
```   

Pour extraire les propriétés de l'objet `adresse` imbriqué dans `personne`, vous pouvez utiliser la syntaxe de déstructuration :  
```js
let { nom, age, adresse: { rue, ville, codePostal } } = personne;

console.log(nom); // Affiche 'Alice'
console.log(age); // Affiche 25
console.log(rue); // Affiche '123 Rue de Paris'
console.log(ville); // Affiche 'Paris'
console.log(codePostal); // Affiche '75001'

// Autre Exemple
const LOCAL_FORECAST = {
    today: { min:72, max:83 },
    tomorrow:{min:73.3, max: 84.6}
};

function gerMaxOfTomorrow (forecast){
    "use strict"; 
    const {tomorrow :{ max : max0fTomorrow } } = forecast; 
    //la valeur de la propriété max équivaut à celle de la variable
    return max0fTomorrow;
}

console.log(gerMaxOfTomorrow(LOCAL_FORECAST));
```  
Que retourne ce code ❓  

### Renommage des variables
Vous pouvez également renommer les variables lors de la déstructuration :  
```js
let { nom: n, age: a, adresse: { rue: r, ville: v, codePostal: cp } } = personne;

console.log(n); // Affiche 'Alice'
console.log(a); // Affiche 25
console.log(r); // Affiche '123 Rue de Paris'
console.log(v); // Affiche 'Paris'
console.log(cp); // Affiche '75001'

```

### Valeurs par défaut
Vous pouvez définir des valeurs par défaut pour les variables au cas où certaines propriétés ne seraient pas présentes dans l'objet :  
```js
let personne = {
    nom: 'Alice',
    adresse: {
        ville: 'Paris'
    }
};

let { nom, age = 30, adresse: { rue = 'N/A', ville, codePostal = '00000' } } = personne;

console.log(nom); // Affiche 'Alice'
console.log(age); // Affiche 30 (valeur par défaut)
console.log(rue); // Affiche 'N/A' (valeur par défaut)
console.log(ville); // Affiche 'Paris'
console.log(codePostal); // Affiche '00000' (valeur par défaut)

```  

### Déstructuration dans les paramètres de fonction 
La déstructuration des objets imbriqués peut également être utilisée directement dans les paramètres de fonction :  
```js
function afficherPersonne({ nom, age = 30, adresse: { rue = 'N/A', ville, codePostal = '00000' } }) {
    console.log(`Nom : ${nom}, Age : ${age}`);
    console.log(`Adresse : ${rue}, ${ville}, ${codePostal}`);
}

let personne = {
    nom: 'Alice',
    adresse: {
        ville: 'Paris'
    }
};

afficherPersonne(personne);
// Affiche :
// Nom : Alice, Age : 30
// Adresse : N/A, Paris, 00000

//  Exemple2

const stats = { 
    max:56.78,
    standard_deviation:4.34,
    median:34.54,
    mode:23.87,
    min:-0.75,
    average:35.85
};

const half = (function () {
    return function half({max,min}) {
        return (max + min) / 2.0 ;
    };
})();

console.log(stats);
console.log(half(stats));
```  

### destructuration avec le rest opérator 
```js
const source = [1,2,3,4,5,6,7,8,9,10];

function removeFirtstTwo(list) {
    const [,,,...arr] = list; //arr c'est tout le reste du tableau affecté sauf les trois premiers
    return arr; 
}
const arr = removeFirtstTwo(source);
console.log(arr);//[5,6,7,8,9,10]
console.log(source);// [1,2,3,4,5,6,7,8,9,10]
```  
ce script extrait les éléments restants d'un tableau après avoir ignoré les deux premiers éléments et stocke ces éléments dans un nouveau tableau, sans modifier le tableau d'origine.