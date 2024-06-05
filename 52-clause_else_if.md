# Clause else if
Considérons les conditions suivantes :   
Prenons le cas où nous devons comparer un nombre par rapport à `10` et `5` et déterminer où il se situe par rapport à cet intervalle.

```js
    const val = 6;

    if(val < 5)
    {
        console.log("La valeur est plus petite que 5");
    } else {
        console.log("La valeur est plus grande que 5");
    }
```

La condition ci-dessus est valide mais l'objectif ici est de déterminer la position d'une valeur par rapport à l'intervalle défini par 5 et 10. La valeur est-elle avant, entre ou après l'intervalle ? Dans un tel cas, nous pouvons recourir à la clause `else if`.

```js
    if(val < 5) //(`if` pour dire `si`)
    {
        console.log("La valeur est située avant l'intervalle défini par 5 et 10");
    } 
    else if (val > 10) //(`else if` pour dire `sinon si`)
    {
        console.log("La valeur est située après l'intervalle défini par 5 et 10");
    } 
    else //(`else` pour dire `sinon`)
    {
        console.log("La valeur est située à l'intérieur l'intervalle défini par 5 et 10");
    }
```