# Fonction parseInt
La fonction `parseInt()` analyse une chaîne de caractère fournie en argument et renvoie un entier.

* Syntaxe :

```js
    parseInt(string, radix)
```

- `string` : C'est la chaîne de caractères que vous souhaitez convertir en entier.
- `radix` : C'est une valeur optionnelle comprise entre `2` et `36` qui spécifie la base numérique à utiliser lors de la conversion. Si cette valeur n'est pas fournie, parseInt() supposera une base décimale.

Exemples : 

```js
    // Exemple 1: Chaîne commençant par des chiffres et contenant des lettres
    let num1 = parseInt("123abc"); // num1 vaut 123
    console.log(num1); // Affiche: 123

    // Exemple 2: Chaîne commençant par des lettres
    let num2 = parseInt("abc123"); // num2 vaut NaN (Not a Number)
    console.log(num2); // Affiche: NaN

    // Exemple 3: Chaîne commençant par des symboles
    let num3 = parseInt("$123"); // num3 vaut NaN (Not a Number)
    console.log(num3); // Affiche: NaN

    // Exemple 4: Chaîne commençant par des espaces, puis des chiffres
    let num4 = parseInt("   456"); // num4 vaut 456 (les espaces en début de chaîne sont ignorés)
    console.log(num4); // Affiche: 456

    // Exemple 5: Chaîne contenant des chiffres, des symboles, et des lettres
    let num5 = parseInt("789#abc"); // num5 vaut 789 (s'arrête au premier symbole non valide)
    console.log(num5); // Affiche: 789

    // Exemple 6: Chaîne contenant uniquement des symboles
    let num6 = parseInt("!!!"); // num6 vaut NaN (aucun chiffre valide trouvé)
    console.log(num6); // Affiche: NaN

    // Exemple 7: Chaîne contenant un mélange de caractères avec un radix spécifié
    let num7 = parseInt("1A", 16); // num7 vaut 26 (1A interprété comme un nombre hexadécimal)
    console.log(num7); // Affiche: 26

    // Exemple 8: Chaîne avec des caractères non numériques et un radix binaire
    let num8 = parseInt("1010b", 2); // num8 vaut 10 (s'arrête au premier caractère non valide 'b')
    console.log(num8); // Affiche: 10

    // Exemple 9: Chaîne vide
    let num9 = parseInt(""); // num9 vaut NaN (chaîne vide)
    console.log(num9); // Affiche: NaN

    // Exemple 10: Chaîne contenant des chiffres et des espaces
    let num10 = parseInt("123 456"); // num10 vaut 123 (s'arrête au premier espace)
    console.log(num10); // Affiche: 123


```