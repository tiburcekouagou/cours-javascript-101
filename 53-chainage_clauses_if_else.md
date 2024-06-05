# Chainage dans les clauses if...else

Il est possible de chaîner des clauses `if...else` 

Considérons les conditions suivantes : 

```
si num < 5    ====> console.log("Tiny");
si num < 10   ====> console.log("Small");
si num < 15   ====> console.log("Medium");
si num < 20   ====> console.log("Large");
si num >= 20  ====> console.log("Huge");
```

la chaînage donnera le bloc de code suivant : 

```js
    if(num < 5){
        console.log("Tiny");
    } else if(num < 10) {
        console.log("Small");
    } else if (num < 15){
        console.log("Medium");
    } else if (num < 20) {
        console.log("Large");
    } else {
        console.log("Huge");
    }
```