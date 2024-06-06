# 72 - Record Collection
Vous créez une fonction qui facilite la maintenance d'une collection d'albums musicaux. La collection est organisée comme un objet contenant plusieurs albums qui sont également des objets. Chaque album est représenté dans la collection avec un nom id de propriété unique. Dans chaque objet album, il existe diverses propriétés décrivant des informations sur l'album. Tous les albums ne contiennent pas des informations complètes.

## Exercice:
La fonction `updateRecords` prend `4` arguments représentés par les paramètres de fonction suivants :

 * `records`- un objet contenant plusieurs albums individuels
 * `id`- un numéro représentant un album spécifique dans l' recordsobjet
 * `prop`- une chaîne représentant le nom de la propriété de l'album à mettre à jour
 * `value`- une chaîne contenant les informations utilisées pour mettre à jour la propriété de l'album

```js
const recordCollection = {
    2548: {
        albumTitle: 'Slippery When Wet',
        artist: 'Bon Jovi',
        tracks: ['Let It Rock', 'You Give Love a Bad Name']
    },
    2468: {
        albumTitle: '1999',
        artist: 'Prince',
        tracks: ['1999', 'Little Red Corvette']
    },
    1245: {
        artist: 'Robert Palmer',
        tracks: []
    },
    5439: {
        albumTitle: 'ABBA Gold'
    }
};
        
function updateRecords(records, id, prop, value) {
    // ...
    return records;
}
```
Complétez la fonction en utilisant les règles ci-dessous pour modifier l'objet passé à la fonction.

=> Votre fonction doit toujours renvoyer l'objet records entier.   
=> Si `value` est une chaîne vide, supprimez la propriété prop donnée de l'album.   
=> Si `prop` n'est pas egale tracks et `value` n'est pas une chaîne vide, attribuez `value` au fichier prop.   
=> Si `prop` est trackset value n'est pas une chaîne vide, mais que l'album n'a pas de trackspropriété, créez un tableau vide et ajoutez value -le.   
=> Si prop est trackset value n'est pas une chaîne vide, ajoutez-la value à la fin du tableau existant de l'album tracks.   
=> Remarque : Une copie de l' recordCollectionobjet est utilisée pour les tests. Vous ne devez pas modifier directement l' record Collectionobjet.   

    
## SOLUTION

```js
const recordCollection = {
    2548: {
        albumTitle: 'Slippery When Wet',
        artist: 'Bon Jovi',
        tracks: ['Let It Rock', 'You Give Love a Bad Name']
    },
    2468: {
        albumTitle: '1999',
        artist: 'Prince',
        tracks: ['1999', 'Little Red Corvette']
    },
    1245: {
        artist: 'Robert Palmer',
        tracks: []
    },
    5439: {
        albumTitle: 'ABBA Gold'
    }
};
        
function updateRecords(records, id, prop, value) {
  if (value === '') {
    delete records[id][prop];
  } else if (prop === "tracks") {
    records[id][prop] = records[id][prop] || [];
    records[id][prop].push(value);
  } else {
    records[id][prop] = value;
  }
  return records;
}
        
updateRecords(recordCollection, 5439, 'artist', 'ABBA');
```