# 79 - Do...while loops
Le prochain type de boucle que vous apprendrez s’appelle une boucle `do...while`. On l'appelle une boucle `do...while` car elle fera d'abord dépasser le code à l'intérieur de la boucle quoi qu'il arrive, puis continuera à exécuter la boucle `while` à laquelle la condition spécifiée est évaluée `true`.

## Exemple 1:
Nous allons commencer à `i = 10` et boucler while `i > 0`. Nous allons décrémenter `i` de `2` chaque boucle avec `i -= 2`.

```js
    const ourArray = [];
    let i = 0;

    do {
        ourArray.push(i);
        i++;
    } while (i < 5);
```
L'exemple ci-dessus se comporte de la même manière que les autres types de boucles et le tableau résultant ressemblera à `[0, 1, 2, 3, 4]`.

## Exemple 2 :
Cependant, ce qui différencie `do...while` des autres boucles est la façon dont elle se comporte lorsque la condition échoue lors de la première vérification. Voyons cela en action. Voici une boucle while régulière qui exécutera le code dans la boucle tant que `i < 5` :

```js
        const ourArray = []; 
        let i = 5;

        while (i < 5) {
        ourArray.push(i);
        i++;
        }
```
Dans cet exemple, nous initialisons la valeur de ourArray à un tableau vide et la valeur de `i` à `5`. Lorsque nous exécutons la boucle while, la condition est évaluée à false car `i` n'est pas inférieur à `5`, nous n'exécutons donc pas le code à l'intérieur de la boucle. Le résultat est  qu'à ourArray aucune valeur n'y sera ajoutée, et cela ressemblera toujours à `[]` jusqu'à ce que tout le code de l'exemple ci-dessus termine son exécution. Maintenant, jetez un œil à une boucle `do...while` :

```js
        const ourArray = []; 
        let i = 5;

        do {
        ourArray.push(i);
        i++;
        } while (i < 5);
```
Dans ce cas, nous initialisons la valeur de `i` à `5`, comme nous l'avons fait avec la boucle while. Lorsque nous arrivons à la ligne suivante, il n'y a aucune condition à évaluer, nous allons donc au code entre les accolades et l'exécutons. Nous allons ajouter un seul élément au tableau, puis incrémenter i avant de passer à la vérification des conditions. Lorsque nous évaluons enfin la condition `i < 5` sur la dernière ligne, nous voyons que i est maintenant à 6, ce qui échoue à la vérification conditionnelle, nous quittons donc la boucle et avons terminé. À la fin de l’exemple ci-dessus, la valeur de ourArray est `[5]`. Essentiellement, une boucle do...while garantit que le code à l’intérieur de la boucle s’exécutera au moins une fois. 

## Exercice:
Essayons de faire fonctionner une boucle `do...while` en poussant les valeurs vers un tableau. 
Changez la boucle while dans le code en boucle do...while afin que la boucle pousse uniquement le nombre 10 vers myArray et que i soit égal à 11 à la fin de l'exécution de votre code.

```js
        const myArray = [];
        let i = 10;

        //...

        while (i < 5) {
        myArray.push(i);
        i++;
        }     
```
        Vous devriez utiliser une boucle do...while pour cet exercice.
        myArray devrait être égal à [10].
        i devrait être égal 11

## SOLUTION

```js
    const myArray = [];

    let i = 10;

    do {
        myArray.push(i);
        i++;
    } while (i < 10);
```