## Modifier les données d'un tableau
```js
let fruits = ["pomme", "banane", "cerise"]; 
fruits[0] = "avocat"; // Notre tableau vaudra maintenant ["avocat", "banane", "cerise"]
fruits[5] = "papaye"; // Notre tableau vaudra désormais ["avocat", "banane", "cerise", undefined, undefined, "papaye"]
```

**NB**: le tableau `fruits` est modifié pour inclure des valeurs `'undefined'` aux indices `3` et `4`, car ils n'ont pas été explicitement définis., mais il est important de noter que la création de `"trous"` dans un tableau (indices non définis) peut parfois conduire à des comportements inattendus ou à des difficultés lors de la manipulation du tableau.
