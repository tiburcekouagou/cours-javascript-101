# Générer des fractions aléatoires 
La fonction `Math.random()` renvoie un nombre  aléatoire compris dans l'intervalle `[0, 1[` (`0` est compris dans l'intervalle mais `1` en est exclu).

- En combinaison avec la fonction `Math.floor()` et en faisant preuve d'ingéniosité, il est possible de générer uniquement des entiers.
Rappel : la fonction `Math.floor()` renvoie le plus grand entier qui est inférieur ou égal à la valeur qu'on lui passe en paramètre.

## Exemples : 

```js
    console.log(Math.random()) // => génération de nombre aléatoire compris entre 0 et 1(exclu)
    console.log(Math.floor(Math.random() * 20)) //=> retourne des entiers compris entre 0 et 20 (exclu)
    console.log(Math.floor(Math.random() * 20 + 1)) //=> retourne des entier compris entre 0 et 20 (compris)
```

- Il est possible de spécifier un intervalle entre lequel les nombres aléatoires doivent être générés
Consisdérons les valeurs suivantes : `10` et `15`. l'objectif est de générer des nombres compris entre ces deux valeurs.

```js
    console.log(Math.random()) // => génération de nombre aléatoire compris entre 0 et 1(exclu)
    console.log(Math.floor(Math.random() * (15 - 10))) // => génération de nombre entier aléatoire compris entre 0 et 5 (exclu. 5 étant la différence entre 15 et 10)
    console.log(Math.floor(Math.random() * (15 - 10 + 1))) // => génération de nombre entier aléatoire compris entre 0 et 5 (5 inclu)
    console.log(Math.floor(Math.random() * (15 - 10 + 1)) + 10) // => génération de nombre entier aléatoire compris entre 10 (0 + 10) et 15 (5 + 10) avec '15' inclu dans l'intervalle
```