## Ecrire du code reutilisable grâce aux fonctions

Les fonctions sont des blocs de code réutilisables qui effectuent une tâche spécifique.
Elles permettent de:  
- Réduire la répétition de code.
- Faciliter la maintenance et le débogage.
- Améliorer la lisibilité et la modularité du code.
- Réutiliser du code dans différentes parties de l'application.

## Définition et Utilisation des Fonctions
### Définir une Fonction
Voici la syntaxe de base pour définir une fonction en JavaScript :
```js
function nomDeLaFonction() {
  // Corps de la fonction
  console.log('Un sourire ne coûte rien mais il crée beaucoup.');
}
```
Décomposons un peu ce charabia

## le mot-clé `function` :
est utilisé pour déclarer une nouvelle fonction et indique donc au moteur JavaScript que vous êtes entrain de définir une fonction.
## `nomDeLaFonction` :
Le nom que vous donnez à la fonction.
Doit être unique dans le même scope (portée).
Utilisé pour appeler ou invoquer la fonction plus tard.
## les parenthèses :
les parenthèses vont permettre de passer plus tard des paramètres à notre fonction. Ces paramètres seront ensuite utilisés dans le corps de la fonction.
## Accolades { } :
Elle délimitent le corps de la fonction et contiennent les instructions, c'est à dire ce que la fonction est censée faire.
## Corps de la fonction :
Les instructions à exécuter lorsque la fonction est appelée.
Peut inclure des déclarations de variables, des boucles, des conditions, et d'autres appels de fonctions.

## Appeler une fonction 📣📣
Une fois que vous avez défini votre fonction, cela reste juste une définition, rien ne se passe dans le code. Le corps de votre fonction ou les instructions de votre fonction seront exécutées uniquement lorsque vous faites appel à cette fonction. 
Pour appeler votre fonction afin qu'elle s'exécute, vous écrivez le nom que vous avez donné à votre fonction suivi des parenthèses.
Prenons le cas de notre fonction définit plus haut. Pour appeler cette fonction, on fera ceci:
```js
nomDeLaFonction(); //ce qui affiche => Un sourire ne coûte rien mais il crée beaucoup.

💡💡 //IL ne faut pas oublier la parenthèse 
```