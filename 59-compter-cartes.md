# Fonction de Comptage de Cartes pour le Blackjack en JavaScript

Le `Blackjack`, également connu sous le nom de `21`, est un jeu de cartes populaire joué dans les casinos du monde entier. L'objectif du jeu est de battre le croupier en ayant une main dont la valeur est plus proche de `21` sans dépasser ce nombre.

## Règles de Base du Blackjack
### Valeur des Cartes :

Les cartes de `2` à `10` ont leur valeur faciale.   
Les cartes de figures (Valet, Dame, Roi) valent `10` points.
L'As vaut `1` ou `11` points, selon ce qui est le plus avantageux pour la main.

### Déroulement du Jeu :
Chaque joueur commence avec deux cartes visibles, tandis que le croupier reçoit une carte visible et une carte cachée.  
Les joueurs ont le choix de "tirer" (prendre une autre carte) ou de "rester" (conserver leur main actuelle).  
Les joueurs peuvent également doubler leur mise initiale ou se séparer en deux mains s'ils ont une paire.  
Une fois que tous les joueurs ont terminé leur tour, le croupier révèle sa carte cachée et continue de tirer des cartes jusqu'à atteindre une valeur de 17 ou plus.

### Conditions de Victoire :
Si la main d'un joueur dépasse `21`, il "saute" et perd sa mise.  
Si la main d'un joueur est plus proche de `21` que celle du croupier sans dépasser `21`, le joueur gagne.   
Si la main du croupier dépasse `21`, tous les joueurs restants gagnent.   
Si un joueur a exactement `21` avec ses deux premières cartes (un As et une carte valant `10`), c'est un `Blackjack` et le joueur gagne `1,5` fois sa mise, sauf si le croupier a aussi un `Blackjack`, ce qui conduit à une égalité.

## Comptage de Cartes
Le `comptage de cartes` est une technique utilisée dans le `blackjack` pour suivre les cartes hautes et basses qui restent dans le sabot. Cette technique aide les joueurs à prendre des décisions éclairées sur leurs mises. Nous allons créer une fonction de comptage de cartes en JavaScript.

### Règles de Base du Comptage de Cartes
Dans le système `Hi-Lo` (le plus couramment utilisé), on attribut aux cartes des valeurs spécifiques :

Cartes de 2 à 6 : +1  
Cartes de 7 à 9 : 0  
Cartes de 10, J, Q, K, A : -1  
Le compte commence à `0` et est ajusté à chaque carte tirée. Un compte élevé indique qu'il reste plus de cartes hautes dans le sabot, avantageant le joueur.

## Implémentation de la Fonction
Nous allons implémenter une fonction de comptage de cartes qui :
👉 Met à jour le compte basé sur les valeurs des cartes.
👉 Retourne le compte courant et une recommandation pour miser ("Bet") ou passer ("Hold").

On peut le faire de plusieurs façon, mais on utilisera les switch case ici.
```js
        let compteur = 0; //Initialisation du compteur
       function compterCarte(carte) {
            switch(carte) {
                case 2:
                case 3:
                case 4:
                case 5:
                case 6:
                    compteur++; //Incrémentation du compteur
                    break;
                case 10:
                case "J":
                case "Q":
                case "K":
                case "A":
                    compteur--; //Décrementation du compteur
                    break;
            }

            let action = "Mise"; //Initialisation de la variable servant à dire si le joueur veux miser ou non
            if (compteur > 0) {
                action = "Ne mise pas"; //Changement de la valeur en fonction du la valeur de compteur
            }

            return compteur + " " + action; //la valeur de retour
       }

// Exemples d'utilisation
let result;

result = compterCarte(2);
console.log(result); // Attendu : "1 Bet"

result = compterCarte('K');
console.log(result); // Attendu : "0 Hold"

result = compterCarte(5);
console.log(result); // Attendu : "1 Bet"

result = compterCarte(10);
console.log(result); // Attendu : "0 Hold"

result = compterCarte('A');
console.log(result); // Attendu : "-1 Hold"
```