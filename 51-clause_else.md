# Clause else 
Considérons les conditions suivantes : 

```js
    const val = 6;

    if(val > 5){
        console.log("La valeur est plus grande que 5");
    }

    if(val < 5){
        console.log("La valeur est plus petite que 5");
    }
```

L'objectif ici étant d'effectuer la comparaison d'une variable par rapport à `5` et de dire si oui ou non elle en est supérieure, il est possible de possible de combiner les deux conditions ci-dessus en un seul bloc de code en faisant intervenir la clause `else`

```js
    if (val > 5) //(`if` pour dire `si`)
    { 
        console.log("La valeur est plus grande que 5");
    } 
    else //(`else` pour dire `sinon`)
    { 
        console.log("La valeur est plus petite que 5");
    }
```