# mot clé const


Le mot-clé `const` en JavaScript, introduit avec `ECMAScript 6 (ES6)` en 2015, est utilisé pour déclarer des variables dont la valeur ne peut pas être réassignée une fois définie. Caractéristiques et  comportement de `const` :

## 1. Déclaration et Initialisation

### Déclaration
Une variable déclarée avec `const` doit être initialisée au moment de la déclaration. Si vous ne le faites pas, une erreur de syntaxe se produira.

```js
    const a = 10;
    console.log(a); // 10

    const b; // SyntaxError: Missing initializer in const declaration
```
## 2. Immuabilité de la Référence

### - Immuabilité
Le mot-clé `const` empêche la réaffectation de la variable. Une fois qu'une variable est déclarée avec `const`, vous ne pouvez pas lui attribuer une nouvelle valeur.

```js
    const c = 20;
    c = 30; // TypeError: Assignment to constant variable.
```
## 3. Portée (Scope)

### Portée de bloc
Comme `let`, `const` a une portée de bloc, ce qui signifie que la variable est accessible uniquement dans le bloc où elle est déclarée (entre {}).

```js
    if (true) {
        const d = 40;
        console.log(d); // 40
    }
    console.log(d); // ReferenceError: d is not defined
```
## 4. Const et Objets

### Objets
Bien que const empêche la réaffectation de la variable, il ne rend pas l'objet lui-même immuable. Les propriétés de l'objet peuvent toujours être modifiées.

```js
    const obj = { name: "Alice" };
    obj.name = "Bob"; // Ceci est permis
    console.log(obj.name); // "Bob"

    obj = { name: "Charlie" }; // TypeError: Assignment to constant variable.
```
### Tableaux
De même, les tableaux déclarés avec const peuvent être modifiés, mais leur référence ne peut pas être réassignée.

```js
    const arr = [1, 2, 3];
    arr.push(4); // Ceci est permis
    console.log(arr); // [1, 2, 3, 4]

    arr = [5, 6, 7]; // TypeError: Assignment to constant variable.
```


## 5. Hoisting (Élévation)

### Hoisting avec const
Comme `let`, les variables déclarées avec `const` sont élevées (hoisted) au sommet de leur portée, mais elles ne sont pas initialisées. Les utiliser avant leur déclaration entraîne une erreur `ReferenceError`.

```js
    console.log(e); // ReferenceError: Cannot access 'e' before initialization
    const e = 50;
    console.log(e); // 50
```

## 6. Bonnes pratiques

### Utilisation de `const`

- Préférence pour `const` : Il est généralement recommandé d'utiliser `const` par défaut, sauf si vous savez que la variable doit être réassignée. Cela rend votre code plus prévisible et plus facile à comprendre.

- `let` pour les variables réassignables : Utilisez `let` uniquement pour les variables dont la valeur peut changer.

## Exemple complet

```js
    // Déclaration avec const
    const PI = 3.14;
    console.log(PI); // 3.14

    // Essayez de réassigner une variable const (cela génère une erreur)
    PI = 3.14159; // TypeError: Assignment to constant variable.

    // Utilisation de const avec des objets
    const person = { name: "Alice" };
    person.name = "Bob"; // Ceci est permis
    console.log(person.name); // "Bob"

    // Essayez de réassigner l'objet (cela génère une erreur)
    person = { name: "Charlie" }; // TypeError: Assignment to constant variable.

    // Utilisation de const avec des tableaux
    const numbers = [1, 2, 3];
    numbers.push(4); // Ceci est permis
    console.log(numbers); // [1, 2, 3, 4]

    // Essayez de réassigner le tableau (cela génère une erreur)
    numbers = [5, 6, 7]; // TypeError: Assignment to constant variable.
```