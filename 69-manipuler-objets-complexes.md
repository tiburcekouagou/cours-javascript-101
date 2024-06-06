# 69 - Manipuler les Objets Complexes
Parfois, vous souhaiterez peut-être stocker des données dans une structure de données flexible . Un objet JavaScript est un moyen de gérer des données flexibles. Ils permettent des combinaisons arbitraires de chaînes , de nombres , de booléens , de tableaux , de fonctions et d'objets.

## Exemple 1:
Voici un exemple de structure de données complexe :

```js
        const ourMusic = [
            {
                "artist": "Daft Punk",
                "title": "Homework",
                "release_year": 1997,
                "formats": ["CD", "Cassette", "LP" ],
                "gold": true
            }
        ];
```
Il s'agit d'un tableau qui contient un objet à l'intérieur. L'objet contient diverses métadonnées sur un album. Il possède également un formats tableau imbriqué. Si vous souhaitez ajouter d'autres enregistrements d'album, vous pouvez le faire en ajoutant des enregistrements au tableau de niveau supérieur. Les objets contiennent des données dans une propriété qui a un format clé-valeur. Dans l'exemple ci-dessus, "artist": "Daft Punk"est une propriété qui a une clé artist et une valeur de Daft Punk.

**Remarque** : Vous devrez placer une virgule après chaque objet du tableau, sauf s'il s'agit du dernier objet du tableau.

## Exemple 2:
Ajoutez un nouvel album au tableau myMusic. Ajoutez artist des title chaînes, release_year un nombre et un formats tableau de chaînes.

```js
        const myMusic = [
            {
                "artist": "Billy Joel",
                "title": "Piano Man",
                "release_year": 1973,
                "formats": ["CD", "8T", "LP"],
                "gold": true
            }
        ];
```

`myMusicdevrait` être un tableau   
`myMusicdevrait` avoir au moins deux éléments   
Les éléments du tableau `myMusic` doivent être des objets   
Votre objet `myMusicdoit` avoir au moins `4` propriétés   
Votre objet `myMusicdoit` contenir la propriété `artist` qui est une chaîne   
Votre objet `myMusicdoit` contenir la propriété `title` qui est une chaîne   
Votre objet `myMusicdoit` contenir la propriété `release_year` qui est un nombre   
Votre objet `myMusicdoit` contenir une propriété `formats` qui est un tableau   
`formats` doit être un tableau de chaînes avec au moins deux éléments   
Soit : 

```js
const myMusic = [
    {
            "artist": "Billy Joel",
            "title": "Piano Man",
            "release_year": 1973,
            "formats": [
            "CD",
            "8T",
            "LP"
            ],
            "gold": true
    },
    {
            "artist": "Jack Sparrow",
            "title": "Pirate des Caraïbes",
            "release_year": 2003,
            "formats": [
            "CD",
            "480px",
            "4k"
            ],
    }
];
```
`checkObj({gift: "pony", pet: "kitten", bed: "sleigh"}, "gift")` devrait renvoyer la chaîne `pony`.   
`checkObj({gift: "pony", pet: "kitten", bed: "sleigh"}, "pet")` devrait renvoyer la chaîne `kitten`.   
`checkObj({gift: "pony", pet: "kitten", bed: "sleigh"}, "house")` devrait renvoyer la chaîne `Not Found`.   
`checkObj({city: "Seattle"}, "city")` devrait renvoyer la chaîne `Seattle`.   
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