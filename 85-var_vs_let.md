# var vs let

`var` et `let` sont des instructions qui permettent de déclarer des variables. l'instruction `let` est apparue avec le `ECMAScript 2015` et les différences à noter entre les deux instructions sont les suivantes : 

## 1. Portée (Scope)

### `var`
- **Portée globale ou fonctionnelle** : Une variable déclarée avec `var` est disponible dans toute la fonction où elle est déclarée. Si elle est déclarée en dehors de toute fonction, elle est disponible partout dans le script.

```js
function testVar() {
    if (true) {
        var x = 10;
    }
    console.log(x); // 10 - x est accessible ici
}
testVar();

var y = 20;
console.log(y); // 20 - y est accessible partout dans le script
```

### `let`  
- **Portée de bloc** : Une variable déclarée avec let est disponible uniquement dans le bloc de code où elle est déclarée (entre {}).

```js
function testLet() {
    if (true) {
        let z = 30;
    }
    console.log(z); // ReferenceError: z is not defined - z n'est pas accessible ici
}
testLet();

let w = 40;
console.log(w); // 40 - w est accessible partout dans le script mais pas attaché à l'objet global
```


## 2. Hoisting (Élévation)

### `var`
- `Hoisting avec initialisation` : Les variables déclarées avec var sont déplacées en haut de leur portée et initialisées avec undefined.

```js
console.log(a); // undefined - a est élevé mais non encore assigné
var a = 5;
console.log(a); // 5
```

### `let`
- `Hoisting sans initialisation` : Les variables déclarées avec let sont également déplacées en haut de leur portée, mais ne sont pas initialisées. Les accéder avant leur déclaration génère une erreur.

```js
    console.log(b); // ReferenceError: b is not defined - b est élevé mais non initialisé
    let b = 10;
    console.log(b); // 10
```

## 3. Redéclaration

### `var`
- ``Peut être redéclaré`` : Vous pouvez redéclarer une variable avec var sans erreur.

```js
    var c = 1;
    var c = 2;
    console.log(c); // 2
```

### `let`
- ``Ne peut pas être redéclaré`` : Vous ne pouvez pas redéclarer une variable avec let dans la même portée.

```js
    let d = 1;
    let d = 2; // SyntaxError: Identifier 'd' has already been declared
```

## 4. Objet global

### `var`
- ``Ajout à l'objet global`` : Les variables déclarées avec var au niveau global deviennent des propriétés de l'objet global (comme window dans les navigateurs).

```js
    var e = 10;
    console.log(window.e); // 10 - e est une propriété de l'objet global
```

### `let`
- ``Pas d'ajout à l'objet global`` : Les variables déclarées avec let au niveau global ne deviennent pas des propriétés de l'objet global.

```js
    let f = 20;
    console.log(window.f); // undefined - f n'est pas une propriété de l'objet global
```

Pour finir, `let` est souvent préféré car il est plus sûr et évite certaines des erreurs courantes associées à `let`.