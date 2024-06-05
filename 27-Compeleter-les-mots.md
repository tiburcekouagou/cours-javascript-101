## Word Blank (Completez les mots)

```js
function wordBlanks(nom, adjectif, verbe, pronom) {
    // Entrez votre code ci-dessous
    let result = "";

    // Entrez votre code ci-dessus
    return result;
}

// Changer les mots ici pour tester les fonctions
console.log(wordBlanks("chien", "grand", "court", "vite"));
```

Nous allons utiliser notre connaissance des chaînes de caractères pour construire un jeu de mots où nous remplirons des espaces vides avec différents types de mots espérant construire des phrases sensées.

Pour le faire, nous utilisons des fonctions. Nous n'avons pas encore abordé les fonctions. Pour le moment, ne vous inquiétez pas des fonctions car n'est pas le but de cette leçon; mais nous les verrons plus tard. 

Sachez que nous avons une fonction appelée `wordBlanks`. Nous pouvons appeler cette fonction (comme dans la console.log de l'exemple) puis lui passer des paramètres (nom, adjectifs, verbe et pronom).

L'objectif donc ici, est d'utiliser tous les mots que nous passons dans les parenthèse pour faire une phrase cohérente. Nous pouvons voir que la variable `result` est vide au départ. Nous allons la changer en utilisant les mots passés dans les parenthèses puis les afficher dans la console. Voici comment nous allons le faire:

```js
function wordBlanks(nom, adjectif, verbe, pronom) {
    // Entrez votre code ci-dessous
    let result = "";
    result = "Le " + adjectif + nom + verbe + pronom + " dans la rue";
    // Entrez votre code ci-dessus
    return result;
}

// Changer les mots ici pour tester les fonctions
console.log(wordBlanks("chien", "grand", "court", "vite"));

```

On obtient une chaîne de caractère dans la console: `Le grandchiencourtvite dans la rue`.

On peut remarquer l'abscence des espaces dans le resultat final. A vous de jouer et d'en faire une phrase cohérente.

A présent, changez les paramètres de la fonction (les mots entre parenthèse) afin de réussir à avoir des phrases correctes.