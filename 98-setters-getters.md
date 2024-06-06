En JavaScript, une classe est comme un modèle pour créer des objets. Elle définit des propriétés (des caractéristiques) et des méthodes (des actions) que ces objets peuvent avoir.

### Qu'est-ce qu'un getter et un setter ?

- **Getter** : Une méthode utilisée pour lire la valeur d'une propriété.
- **Setter** : Une méthode utilisée pour modifier la valeur d'une propriété.

Utiliser des getters et setters permet de contrôler comment les propriétés sont lues et modifiées.

- **Exemple :**

Prenons un exemple avec une classe `Rectangle` qui a deux propriétés : `largeur` (width) et `hauteur` (height). On va ajouter des getters et setters pour ces propriétés.

```js

    class Rectangle {
        // Le constructeur initialise les propriétés width et height
        constructor(width, height) {
            this._width = width;
            this._height = height;
        }

        // Getter pour la propriété width
        get width() {
            return this._width;
        }

        // Setter pour la propriété width
        set width(newWidth) {

            // On vérifie que la nouvelle largeur est positive
            if (newWidth > 0) 
            { 
                this._width = newWidth;
            } 
            else 
            {
                console.log('Largeur invalide');
            }
        }

        // Getter pour la propriété height
        get height() {
            return this._height;
        }

        // Setter pour la propriété height
        set height(newHeight) {
            // On vérifie que la nouvelle hauteur est positive
            if (newHeight > 0) 
            { 
                this._height = newHeight;
            } 
            else 
            {
                console.log('Hauteur invalide');
            }
        }
    }

    // Utilisation de la classe Rectangle
    const monRectangle = new Rectangle(10, 5);

    console.log(monRectangle.width);  // Affiche: 10
    console.log(monRectangle.height); // Affiche: 5

    monRectangle.width = 20;          // Met à jour la largeur
    console.log(monRectangle.width);  // Affiche: 20

    monRectangle.height = -10;        // Tentative de définir une hauteur non valide
    // Affiche: Hauteur invalide
    console.log(monRectangle.height); // Affiche: 5 (reste inchangé)

```

- **Explications pas à pas**

1. **Définir une Classe `Rectangle`** :

```js
    class Rectangle {
        constructor(width, height) {
            this._width = width;
            this._height = height;
        }
    }
```

- **class Rectangle** : Définit une nouvelle classe appelée `Rectangle`.
- **constructor(width, height)** : Une fonction spéciale qui initialise un nouvel objet avec les valeurs `width` et `height`.

2. **Ajouter un Getter pour `width`** :

```js
    get width() {
        return this._width;
    }
```

- **get width()** : Une méthode pour lire la valeur de `_width`.
- **return this._width** : Retourne la valeur actuelle de `_width`.

3. **Ajouter un Setter pour `width`** :


```js
    set width(newWidth) {
        if (newWidth > 0) {
            this._width = newWidth;
        } else {
            console.log('Largeur invalide');
        }
    }
```


- **set width(newWidth)** : Une méthode pour définir une nouvelle valeur pour `_width`.
- **if (newWidth > 0)** : Vérifie si la nouvelle largeur est positive.
- **this._width = newWidth** : Met à jour la valeur de `_width`.
- **console.log('Largeur invalide')** : Affiche un message si la nouvelle largeur est invalide.

4. Ajouter un Getter et un Setter pour `height` :

- Le processus est similaire à celui de `width`.

5. **Utiliser la Classe Rectangle** :

- **const monRectangle = new Rectangle(10, 5)** : Crée un nouveau rectangle avec une largeur de 10 et une hauteur de 5.
- **console.log(monRectangle.width)** : Affiche la largeur actuelle.
- **monRectangle.width = 20** : Met à jour la largeur à 20.
- **monRectangle.height = -10** : Tente de définir une hauteur non valide, affiche un message d'erreur.