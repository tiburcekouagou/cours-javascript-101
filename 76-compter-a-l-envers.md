# 76 - Compter à l'envers avec la boucle for
Une boucle for peut également compter à rebours, à condition que nous puissions définir les bonnes conditions.
Afin de décrémenter de deux à chaque itération, nous devrons modifier notre initialisation, notre condition et notre expression finale.

- Exemple 1:
Nous allons commencer à i = 10 et boucler while i > 0. Nous allons décrémenter i de 2 chaque boucle avec i -= 2.

    ```js
        const ourArray = [];

        for (let i = 10; i > 0; i -= 2) {
        ourArray.push(i);
        }
    ```
        ourArray contiendra désormais [10, 8, 6, 4, 2]. 

- Exemple 2:
Modifions notre initialisation et notre expression finale afin de pouvoir compter à rebours par deux pour créer un tableau de nombres impairs décroissants.

    ```js
        const myArray = [];
        // ...
    ```
        myArray contiendra désormais [10, 8, 6, 4, 2]. 

SOLUTION

    ```js
        const myArray = [];

        for (let i = 9; i > 0; i -= 2) {
        myArray.push(i);
        }
    ```