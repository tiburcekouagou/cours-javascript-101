Vous savez maintenant que pour déclarer une variable de type string il faut entourer la valeur avec les doubles guillemets("") ou simple guillemets('') ou encore les back ticks(``).

En JavaScript, certaines séquences de caractères ont des significations spéciales. Par exemple, les guillemets doubles (") et simples (') délimitent les chaînes de caractères, et la barre oblique inverse (\) est utilisée pour indiquer des caractères spéciaux. Pour inclure ces caractères dans une chaîne sans perturber le code, nous devons les échapper.
Il arrive des fois que la veuleur de notre string contient des doubles quotes ou guillemets simple.

## Exemple :
```js
let message = "C'est tout "beau" par ici !";
```
Copier et coller ces lignes dans votre fichier javascript => une erreur apparaît

Lorsque vous utiliser les guillemets simple ou double pour définir un string, il est important de faire attention à l'utilisation des ces guilletmets dans le contenu de votre string.

### Les Caractères d'Échappement Communs
Voici une liste des caractères d'échappement les plus courants :

- **`\\`** : Affiche un antislash.
- **`\'`** : Affiche une apostrophe.
- **`\"`** : Affiche des guillemets doubles.
- **`\n`** : Insère une nouvelle ligne.
- **`\r`** : Retour chariot.
- **`\t`** : Insère une tabulation horizontale.
- **`\b`** : Insère un retour arrière.
- **`\f`** : Insère un saut de page.


## Exercice 1 : Afficher une chaîne avec des guillemets
Essayez d'exécuter le code suivant dans votre console JavaScript :
```js
const phrase = "Il a dit, \"Bonjour tout le monde !\"";
console.log(phrase); affichage => Il a dit, "Bonjour tout le monde !"
```
## Exercice 2 : Insérer une nouvelle ligne et une tabulation
Écrivez un code qui affiche une liste de courses sur deux lignes avec une tabulation pour indenter les éléments :

```js
    const listeCourses = "Liste des courses :\n\t- Pommes\n\t- Poires\n\t- Bananes";
    console.log(listeCourses);
```

A l'affichage on à

```sh
    Liste des courses :
    - Pommes
    - Poires
    - Bananes
```

Essayer, amuser vous bien ! 💥💥
