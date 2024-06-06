# Retourner des booléens d'une fonction

Les `booléens` (true/false) sont des valeurs logiques utilisées pour indiquer des conditions vraies ou fausses.

Supposons que vous souhaitez qu'à la fin de l'execution de votre fonction cette dernière vous retourne `vrai` ou `faux` suivant la logique que vous avez définir dans votre fonction.
Vous pouvez vous retrouver à faire un truc du genre :
```js
  function estSuperieur(a, b) {
            if (a > b) {
                return true
            }else {
                return false
            }
        }
    
    console.log(estSuperieur(6, 4))
```
Dans ce exemple, on vérifie si `a` (6) est supérieur à `b` (4), et vu que `6` est supérieur à `4`, notre console affiche `true`.
Rappelez-vous que les opérations de comparaison retourne un `booleen`, c'est-à-dire c'est opération sont évaluées à `true` ou `false`.
Et donc plutôt que d'utiliser un `if` statement dans notre fonction ci, on va juste demander à notre fonction de retourner le resultat de la comparaison `(a > b)`. On aura ceci:
```js
  function estSuperieur(a, b) {
            return a > b;
        }
    
    console.log(estSuperieur(6, 4))
```

Retourner des booléens à partir de fonctions est une pratique courante en JavaScript pour effectuer des vérifications et des validations.

## Exercice 1 : Retourner un Résultat de Calcul
Objectif : Créez une fonction qui prend un nombre en paramètre et retourne son carré.

## Exercice 2 : Vérifier si un Nombre est Pair
Objectif : Créez une fonction qui prend un nombre en paramètre et retourne true si le nombre est pair, false sinon.