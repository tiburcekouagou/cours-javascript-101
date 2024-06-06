# 67 - Utilisation d'objets pour les recherches
Les objets peuvent être considérés comme un stockage `clé/valeur`, comme un dictionnaire. Si vous disposez de données tabulaires, vous pouvez utiliser un objet pour rechercher des valeurs plutôt qu'une instruction `switch` ou une chaîne de `if/else`. Ceci est particulièrement utile lorsque vous savez que vos données d'entrée sont limitées à une certaine plage.

## Exemple 1:
Voici un exemple d’objet article :

```js
    const article = {
        "title": "How to create objects in JavaScript",
        "link": "https://www.freecodecamp.org/news/a-complete-guide-to-creating-objects-in-javascript-b0e2450655e8/",
        "author": "Kaashan Hussain",
        "language": "JavaScript",
        "tags": "TECHNOLOGY",
        "createdAt": "NOVEMBER 28, 2018"
    };

    const articleAuthor = article["author"];
    const articleLink = article["link"];

    const value = "title";
    const valueLookup = article[value];
```
La variable `articleAuthor` est égale à la chaîne `Kaashan Hussain`, `articleLink` est égale à la chaîne `https://www.freecodecamp.org/news/ a-complete-guide-to-creating-objects-in-javascript-b0e2450655e8/` et `valueLookup` est égale à la chaîne `How to create objects in JavaScript`.

## Exemple 2:
Convertissez l'instruction switch en un objet appelé lookup. Utilisez-le pour rechercher val et attribuer la chaîne associée à la result variable.

```js
function phoneticLookup(val) {
    let result = "";

    switch(val) {
        case "alpha":
        result = "Adams";
        break;
        case "bravo":
        result = "Boston";
        break;
        case "charlie":
        result = "Chicago";
        break;
        case "delta":
        result = "Denver";
        break;
        case "echo":
        result = "Easy";
        break;
        case "foxtrot":
        result = "Frank";
    }

    return result;
}

phoneticLookup("charlie");
```

`phoneticLookup("alpha")` devrait être égal à la chaîne `Adams`   
`phoneticLookup("bravo")` devrait être égal à la chaîne `Boston`   
`phoneticLookup("charlie")` devrait être égal à la chaîne `Chicago`   
`phoneticLookup("delta")` devrait être égal à la chaîne `Denver`   
`phoneticLookup("echo")` devrait être égal à la chaîne `Easy`   
`phoneticLookup("foxtrot")` devrait être égal à la chaîne `Frank`   
`phoneticLookup("")` devrait être égal `undefined`   
        
Vous ne devez pas modifier la déclaration `return`   
Vous ne devez pas utiliser d'instructions `case`, `switch` ou `if`

## SOLUTION

```js
    function phoneticLookup(val) {
    let result = "";

    const lookup = {
        "alpha" : "Adams",
        "bravo" : "Boston",
        "charlie" : "Chicago",
        "delta" : "Denver",
        "echo" : "Easy",
        "foxtrot" : "Frank"
    }
    result = lookup[val];
    return result;
    }

    phoneticLookup("charlie");
```