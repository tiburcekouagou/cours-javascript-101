# Ordre logique dans les clauses if...else

L'ordre des conditions dans les clauses `if...else` en JavaScript est très important pour s'assurer que le programme fonctionne correctement. 

```js
    const val = 7;

    if(val < 10) {
        console.log("Moins que 10");
    } else if (val < 5) {
        console.log("Moins que 10");
    } else {
        console.log("supérieur ou égal à 10");    
    }
```


Pour une valeur de `3`, on a un résultat identique à ce que la valeur `7` nous retourne. Ce qui n'est pas tout à fait logique. Pour resoudre ce problème, il faut changer l'order des conditions.

```js
    if(val < 5) {
        console.log("Moins que 5");
    } else if (val < 10) {
        console.log("Moins que 10");
    } else {
        console.log("supérieur ou égal à 10");    
    }
```
