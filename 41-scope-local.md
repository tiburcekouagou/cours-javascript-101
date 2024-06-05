## Scope Local 📛
Le `scope local` se réfère aux variables qui sont accessibles uniquement à l'intérieur d'une fonction ou d'un bloc de code où elles sont déclarées. Les variables locales sont créées lors de l'exécution de la fonction et détruites lorsque la fonction se termine.

### Exemple de Scope Local

```js
function afficherMessage() {
  let message = "Bonjour"; // Variable locale (c'est-à-dire défini à l'intérieur de la fonction)
  console.log(message); // Accessible uniquement à l'intérieur de la fonction, affiche "Bonjour"
}

afficherMessage(); //affiche Bonjour
//Lorsque vous éssayez d'afficher la variable message en dehors de la fonction, vous aurez une erreur
//Essayez !
console.log(message); // Erreur : message is not defined
```
Dans cet exemple, message est une variable locale, accessible uniquement à l'intérieur de la fonction afficherMessage.

## Un autre Exemple : Redéfinir une variable locale avec le même nom qu'une variable globale
**Objectif** : Déclarez une variable locale avec le même nom qu'une variable globale et observez le comportement. Allez-y essayer ce code !

```js
let pays = "France";

function afficherPays() {
  let pays = "Canada";
  console.log("Le pays à l'intérieur de la fonction est : " + pays); // Attendu : "Canada"
}

afficherPays();
console.log("Le pays à l'extérieur de la fonction est : " + pays); // Attendu : "France"
```
Qu'est-ce que vous remarquez ❓❓

## Exercice 1 : Utiliser une variable globale
Objectif : Déclarez une variable globale et utilisez-la dans une fonction.

## Exercice 2 : Utiliser une variable locale
Objectif : Déclarez une variable locale à l'intérieur d'une fonction et tentez de l'accéder à l'extérieur de la fonction.

