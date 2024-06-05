# Clause switch
L'instruction `switch` est utilisée en JavaScript pour effectuer une sélection parmi un ensemble de valeurs possibles. Elle permet d'exécuter différentes actions en fonction de la valeur d'une expression.
## Syntaxe :  

```js
    switch (expression) {
    case valeur1:
        // instructions à exécuter si expression est égale à valeur1
        break;
    case valeur2:
        // instructions à exécuter si expression est égale à valeur2
        break;
    // Ajoutez autant de cas que nécessaire
    default:
        // instructions à exécuter si expression ne correspond à aucune des valeurs précédentes
    }
```

## Exemple 1 : 

Considérons un exemple où nous utilisons switch pour vérifier le jour de la semaine en fonction d'un numéro de jour :

```js
    let jour = 3;
    let nomJour;

    switch (jour) {
    case 1:
        nomJour = "Lundi";
        break;
    case 2:
        nomJour = "Mardi";
        break;
    case 3:
        nomJour = "Mercredi";
        break;
    case 4:
        nomJour = "Jeudi";
        break;
    case 5:
        nomJour = "Vendredi";
        break;
    case 6:
        nomJour = "Samedi";
        break;
    case 7:
        nomJour = "Dimanche";
        break;
    default:
        nomJour = "Jour invalide";
    }

    console.log("Aujourd'hui, c'est " + nomJour + ".");

```
Dans cet exemple, si `jour` est égal à `3`, la variable `nomJour` sera définie sur `"Mercredi"`. Si jour a une valeur différente de `1` à `7`, `default` sera exécuté, et `nomJour` sera définie sur `"Jour invalide"`.

## Exemple 2 :
Imaginons que nous voulions assigner une catégorie à un nombre entier en fonction de sa valeur. Si le nombre est compris entre `1` et `3` inclusivement, il sera considéré comme `"Faible"`. Si le nombre est compris entre `4` et `6` inclusivement, il sera considéré comme `"Moyen"`. Si le nombre est supérieur à `6`, il sera considéré comme `"Élevé"`

```js
let nombre = 5;
let categorie;

switch (nombre) {
  case 1:
  case 2:
  case 3:
    categorie = "Faible";
    break;
  case 4:
  case 5:
  case 6:
    categorie = "Moyen";
    break;
  default:
    categorie = "Élevé";
}

console.log("Le nombre " + nombre + " est de catégorie : " + categorie + ".");
```
Dans cet exemple, les `case` `1`, `2` et `3` ont le même retour `"Faible"`, et les `case` `4`, `5` et `6` ont le même retour `"Moyen"`. Cela évite la répétition de l'assignation de la variable `categorie` pour chaque valeur individuelle, ce qui rend le code plus concis et plus lisible.

Pour finir, retenez que l'instruction `break` est utilisée dans une structure `switch` pour sortir de celle-ci une fois qu'un `case` correspondant a été trouvé et exécuté. Sans `break`, l'exécution du code continuera dans les `case` suivants, ce qui peut entraîner des comportements inattendus. 
