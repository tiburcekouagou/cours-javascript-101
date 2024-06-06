# Retourner de manière anticipée dans une fonction

Retourner de manière anticipée dans une fonction signifie terminer l'exécution de la fonction et renvoyer une valeur avant d'atteindre la fin de la fonction. Cette technique est utile pour gérer les conditions spéciales, simplifier la logique de la fonction, et éviter les exécutions inutiles.

Prenons cet exemple:
```js
    function estSuperieur(a, b) {
            return a / b;
        }

    console.log(estSuperieur(6, 0)) // ici vous allez voir afficher dans la console 'Infinity' parcequ'on est entrain de diviser 6 par 0
```
Pour éviter d'avoir ce comportement, on peut faire une vérification à l'intérieur de notre fonction pour s'assurer que `b` soit supérieur à `0`.

On peut donc faire ceci:
```js
    function estSuperieur(a, b) {
            if (b === 0) {
                return "Calcule impossible";
            }

            return a / b
        }

    console.log(estSuperieur(6, 0)) //affiche "Calcule impossible" dans la console
```
Dans ce exemple, on vérifie si la valeur de `b = 0`. Lorsque cette comparaison est évaluée à vrai (`true`), on dit à notre fonction de retourner le message `"Calcule impossible"`, ce qui provoque la fin de l'execution de la fonction. Donc l'instruction return `a / b` ne sera pas exécutée.


## Syntaxe pour Retourner de manière anticipée
Pour retourner de manière anticipée dans une fonction, vous utilisez le mot-clé return dès que la condition spécifiée est remplie.

## 💡Note:
Toute instruction après le mot clé return ne sera pas exécutée. hey oui 🙂!