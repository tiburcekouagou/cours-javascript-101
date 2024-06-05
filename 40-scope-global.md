## Scope Global et Scope Local en JavaScript

Le concept de **`scope`** (ou portée) en JavaScript détermine l'accessibilité des variables à différentes parties de votre code, autrement dire le concept de scope détermine à quel endroit ou à quelle partie de notre code, tel ou tel variable est accessible. 
Comprendre ce concept est essentiel pour éviter les erreurs de portée et écrire du code clair et maintenable.

## Scope Global ⭕
- Le scope global se réfère aux variables qui sont accessibles partout dans votre code. 
- Une variable a un scope global lorsqu'elle est déclarée en dehors de toute fonction ou bloc de code.

## Exemple de Scope Global
```js
let nomGlobal = "Alice"; // Variable globale

function afficherNom() {
  console.log(nomGlobal); // Accessible dans la fonction
}

afficherNom(); // Affiche "Alice"
console.log(nomGlobal); // Accessible en dehors de la fonction, affiche "Alice"
```
Dans cet exemple, `nomGlobal` est une `variable globale` (c'est-à-dire déclarée hors de la fonction), accessible à la fois à l'intérieur et à l'extérieur de la fonction `afficherNom`.