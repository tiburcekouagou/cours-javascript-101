## Passage d'Arguments dans une Fonction en JavaScript
Les `arguments` sont des valeurs que vous passez à une fonction lors de son appel. Ils permettent à la fonction de recevoir des données et de les utiliser pour exécuter ses tâches. Voici une explication détaillée du passage d'arguments dans une fonction :

## Définition de la Fonction avec Paramètres
Rappelez vous des parenthèses juste après le nom de votre fonction lors de la définition de votre fonction. Et bien, ces parenthéses ne sont pas là pour faire de la déco 😎😁 !
Ces parenthèses vont servi à acceuillir les paramètres de notre fonction.

## Bon maintenant c'est quoi un paramètre ❓❓
- Les paramètres sont des variables spécifiées dans la définition de la fonction.
- Ils agissent comme des placeholders (espaces réservés) pour les valeurs qui seront passées à la fonction.
- Les paramètres existent uniquement dans le contexte de la fonction. Ils sont utilisés comme variables locales à l'intérieur de la fonction pour manipuler les valeurs qui leur sont passées.

Exemple de paramètres :

```js
function additionner(a, b) {
  console.log(a + b);
}
```
Dans cet exemple, `a` et `b` sont des paramètres de la fonction additionner.

Et on remarque bien que l'instruction dans la fonction dit:
affiche moi dans la console la somme de `a + b`.

Donc la mission de cette fonction, c'est de faire la somme de deux nombres, ce qui veut dire que lorsque cette fonction sera appelée, il faut lui fournir deux nombres afin qu'elle accomplisse sa mission (ou sa tâche). Ces deux nombres que vous allez passer à la fonction sont appelés des `arguments`.

## C'est quoi un argument ❓❓
- Les arguments sont les valeurs réelles passées à la fonction lors de son appel. Ils sont assignés aux paramètres correspondants définis dans la fonction.
- Les arguments fournissent les données que la fonction utilisera pour effectuer ses opérations.
- Les arguments sont passés dans les parenthèses lors de l'appel de la fonction.

Exemple d'arguments :

```js
additionner(3, 5);
```
Dans cet exemple 3 et 5 sont des arguments passés à la fonction additionner.

## Un autre exemple
```js
// Définition de la fonction avec des paramètres
function saluer(prenom, nom) {
  console.log("Bonjour, " + prenom + " " + nom + "!");
}

// Appel de la fonction avec des arguments
saluer("Alice", "Dupont"); //affiche => Bonjour Alice Dupont!
```

Alors, deux trois petits exercice pour l'échauffement 😉😉
### Exercice 1 : Addition de Deux Nombres
Objectif : Créez une fonction qui prend deux nombres en paramètres et affiche leur somme.

### Exercice 2 : Conversion Celsius en Fahrenheit
Objectif : Créez une fonction qui convertit une température de Celsius en Fahrenheit. La formule de conversion est (Celsius * 9/5) + 32.

### Exercice 3 : Inversion d'une Chaîne de Caractères
Objectif : Créez une fonction qui prend une chaîne de caractères en paramètre et retourne cette chaîne inversée.

### Exercice 4 : Vérification d'un Palindrome
Objectif : Créez une fonction qui vérifie si une chaîne de caractères est un palindrome (se lit de la même manière de gauche à droite et de droite à gauche).

### Exercice 5 : Compter les Voyelles dans une Chaîne
Objectif : Créez une fonction qui prend une chaîne de caractères en paramètre et retourne le nombre de voyelles (a, e, i, o, u) dans la chaîne.


