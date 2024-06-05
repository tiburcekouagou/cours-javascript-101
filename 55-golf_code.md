# Golf Code
Dans le jeu de golf, le but est d'envoyer une balle dans un trou en utilisant le moins de coups possible. Chaque trou a un `par`, qui représente le nombre de coups standard pour terminer le trou. Voici un exemple :

```
Trou 1 : Par 4
Trou 2 : Par 3
Trou 3 : Par 5
```

Vous devez écrire un script qui prend en compte le nombre de coups d'un joueur pour chaque trou et indique s'il a joué au-dessus, en dessous ou exactement le par pour chaque trou.

```js
    // Scores pour chaque trou
    const scores = [4, 3, 5];

    // Par pour chaque trou
    const par = [4, 3, 5];

    // Vérification pour le trou 1
    const difference1 = scores[0] - par[0];
    if (difference1 < 0) {
        console.log("Trou 1: Vous êtes " + Math.abs(difference1) + " coup(s) en dessous du par.");
    } else if (difference1 > 0) {
        console.log("Trou 1: Vous êtes " + difference1 + " coup(s) au-dessus du par.");
    } else {
        console.log("Trou 1: Vous êtes au par pour ce trou.");
    }

    // Vérification pour le trou 2
    const difference2 = scores[1] - par[1];
    if (difference2 < 0) {
        console.log("Trou 2: Vous êtes " + Math.abs(difference2) + " coup(s) en dessous du par.");
    } else if (difference2 > 0) {
        console.log("Trou 2: Vous êtes " + difference2 + " coup(s) au-dessus du par.");
    } else {
        console.log("Trou 2: Vous êtes au par pour ce trou.");
    }

    // Vérification pour le trou 3
    const difference3 = scores[2] - par[2];
    if (difference3 < 0) {
        console.log("Trou 3: Vous êtes " + Math.abs(difference3) + " coup(s) en dessous du par.");
    } else if (difference3 > 0) {
        console.log("Trou 3: Vous êtes " + difference3 + " coup(s) au-dessus du par.");
    } else {
        console.log("Trou 3: Vous êtes au par pour ce trou.");
    }
```