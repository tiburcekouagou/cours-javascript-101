# Opérateur ternaire multiple

Les `opérateurs ternaires multiples` sont utilisés pour gérer plusieurs conditions en chaînant plusieurs opérateurs ternaires ensemble. Ils permettent d'écrire des conditions complexes de manière concise, bien que cela puisse parfois nuire à la lisibilité si les conditions deviennent trop nombreuses ou compliquées.

## Syntaxe  
La syntaxe de base d'un opérateur ternaire est la suivante :

```js
    condition ? expressionSiVrai : expressionSiFaux;
```

Pour des opérateurs ternaires multiples, on imbrique des opérateurs ternaires les uns dans les autres :

```js
    condition1 ? expressionSiVrai1 
      : condition2 ? expressionSiVrai2 
      : condition3 ? expressionSiVrai3 
      : expressionParDefaut;

```

## Exemples : 

```js

    /**
     * Exemple 1
     * Considérons un exemple où nous attribuons des notes en fonction d'un score :
     */
    let score = 50;
    let grade = score >= 90 ? "A"
            : score >= 80 ? "B"
            : score >= 70 ? "C"
            : score >= 60 ? "D"
            : "F";

    console.log(`La note est ${grade}.`); // Affiche : La note est F.
```

### Décomposition étape par étape

* **Première condition : `score >= 90`**

```js
    let score = 50;
    let grade = score >= 90 ? "A" : "Next";
```
Ici, on vérifie si score est supérieur ou égal à `90`. Si c'est vrai, grade vaut `"A"`, sinon, on passe à la prochaine étape.

Dans ce cas, score est `50`, donc la condition `score >= 90` est fausse. On passe donc à `"Next"`.

* **Deuxième condition : `score >= 80`**

```js
    let score = 50;
    let grade = score >= 80 ? "B" : "Next";
```

Ici, on vérifie si score est supérieur ou égal à 80. Si c'est vrai, grade vaut "B", sinon, on passe à la prochaine étape.

Dans ce cas, score est 50, donc la condition score >= 80 est fausse. On passe donc à "Next".


* **Troisième condition : `score >= 70`**   

```js
        let score = 50;
        let grade = score >= 70 ? "C" : "Next";
        ```
        Ici, on vérifie si score est supérieur ou égal à 70. Si c'est vrai, grade vaut "C", sinon, on passe à la prochaine étape.

        Dans ce cas, score est 50, donc la condition score >= 70 est fausse. On passe donc à "Next".
```
    
* **Quatrième condition : `score >= 60 `**  

```js
    let score = 50;
    let grade = score >= 60 ? "D" : "Next";
```
Ici, on vérifie si score est supérieur ou égal à 60. Si c'est vrai, grade vaut "D", sinon, on passe à la prochaine étape.

Dans ce cas, score est 50, donc la condition score >= 60 est fausse. On passe donc à "Next".

    
* **Condition par défaut :**  

Si aucune des conditions précédentes n'est vraie, grade vaut "F".

```js
    let score = 50;
    let grade = "F"; // résultat final
```