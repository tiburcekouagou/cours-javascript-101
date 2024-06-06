# 74 - for loops
Vous pouvez exécuter le même code plusieurs fois en utilisant une boucle. Le type de boucle JavaScript le plus courant est appelé boucle `for` car il s’exécute un nombre de fois spécifique.
Les boucles `for` sont déclarées avec trois expressions facultatives séparées par des points-virgules:
`for (a; b; c)`, où   
 `a` est l'instruction d'initialisation,   
 `b` est l'instruction de condition et   
 `c` est l'expression finale.

- L'**instruction d'initialisation** est exécutée une seule fois avant le début de la boucle. Il est généralement utilisé pour définir et configurer votre variable de boucle.   
- L'**instruction de condition** est évaluée au début de chaque itération de boucle et continuera tant qu'elle sera évaluée à true. Lorsque la condition est false au début de l’itération, la boucle cessera de s’exécuter. Cela signifie que si la condition commence comme fausse, votre boucle ne s'exécutera jamais.   
- L'**expression finale** est exécutée à la fin de chaque itération de boucle, avant la prochaine vérification de condition et est généralement utilisée pour incrémenter ou décrémenter votre compteur de boucle.

# Exemple:
Dans l'exemple suivant, nous initialisons avec `i = 0` et itérons pendant que notre condition `i < 5` est vraie. Nous incrémenterons `i` à `1` chaque itération de boucle avec `i++` comme expression finale.

```js
        const ourArray = [];

        for (let i = 0; i < 5; i++) {
        ourArray.push(i);
        }
```
`ourArray` aura désormais la valeur `[0, 1, 2, 3, 4]`.

# Exercice:
Utilisez une boucle for pour pousser les valeurs `1` à `5` sur `myArray`.

Soit: 

```js
        const myArray = [];
        // ...
```
Vous devriez utiliser une boucle for pour cela.
`myArray` devrait être égal à `[1, 2, 3, 4, 5]`.

# SOLUTION

```js
        const myArray = [];
        
        for (let i = 1; i <= 5; i++) {
        myArray.push(i);
        }
```