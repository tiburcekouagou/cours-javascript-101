# 70 - Objets imbriqués
Les sous-propriétés des objets sont accessibles en enchaînant la notation par points ou par crochets.

## Exemple 1:
Voici un objet imbriqué :

```js 
    const ourStorage = {
        "desk": {
            "drawer": "stapler"
        },
        "cabinet": {
            "top drawer": { 
            "folder1": "a file",
            "folder2": "secrets"
            },
            "bottom drawer": "soda"
        }
    };

    ourStorage.cabinet["top drawer"].folder2;
    ourStorage.desk.drawer;
```

`ourStorage.cabinet["top drawer"].folder2` sera la chaîne `secrets`, et `ourStorage.desk.drawer` sera la chaîne `stapler`.

## Exercice:
Accédez à l'objet `myStorage` et affectez le contenu de la propriété `"glove box"` à la variable `gloveBoxContents`. Utilisez la notation par points pour toutes les propriétés lorsque cela est possible, sinon utilisez la notation par crochets.

    ```js
        const myStorage = {
            "car": {
                "inside": {
                "glove box": "maps",
                "passenger seat": "crumbs"
                },
                "outside": {
                "trunk": "jack"
                }
            }
        };

        const gloveBoxContents = ?????;
    ```
`gloveBoxContents` devrait être égal à la chaîne `maps`.
Votre code doit utiliser la notation par points, lorsque cela est possible, pour accéder aux propriétés de l'objet `myStorage`.
`gloveBoxContents` doit toujours être déclaré avec const.
Vous ne devez pas modifier l'objet `myStorage`.

## SOLUTION

```js
    const myStorage = {
        "car": {
            "inside": {
            "glove box": "maps",
            "passenger seat": "crumbs"
            },
            "outside": {
            "trunk": "jack"
            }
        }   
    };

    const gloveBoxContents = myStorage.car.inside["glove box"];
```
