# Empêcher la Mutation d'un Objet en JavaScript
En JavaScript, les objets sont par défaut `mutables`, ce qui signifie que leurs propriétés peuvent être modifiées après leur création (mais ça tu le sais déjà).
Et comme on l'a vu précedemment, déclarer un tableau avec `const` n'empêche pas la modification des éléments internes, c'est pareil pour les objets.
Cependant, dans certains cas, il peut être nécessaire d'empêcher la mutation d'un objet afin de garantir l'intégrité des données.

Supposons qu'on à:
```js
const alice = {
    nom: "Doe",
    prenom: "Alice",
    Pays: "Bénin"
}

alice.prenom = "Yasmina"
console.log(alice); //affiche => { nom: "Doe", prenom: "Yasmina", Pays: "Bénin" } et on remarque bien que le prénom à changer
```

Alors voyons un peux ce que javascript nous propose pour empêcher la mutation d'un objet

## Techniques pour Empêcher la Mutation d'un Objet

* **Object.freeze()** :
Rend un objet entièrement immuable, empêchant l'ajout, la suppression et la modification de ses propriétés.

## Exemple:
```js
const voiture = {
  marque: 'Toyota',
  modele: 'Corolla',
  annee: 2020
};

Object.freeze(voiture); //Object.freeze() prends en paramètre l'objet dont on veut empêcher la mutation

voiture.marque = 'Honda'; // Ignoré, ne modifie pas l'objet
voiture.couleur = 'rouge'; // Ignoré, ne peut pas ajouter de nouvelles propriétés
delete voiture.modele; // Ignoré, ne peut pas supprimer de propriétés

console.log(voiture); // Attendu : { marque: 'Toyota', modele: 'Corolla', annee: 2020 }
```

* **Object.seal()** :
Empêche l'ajout ou la suppression de propriétés, mais permet toujours la modification des propriétés existantes.
## Exemple:
```js
const utilisateur = {
  nom: 'Alice',
  age: 25
};

Object.seal(utilisateur); //bject.seal() prends en paramètre l'objet dont on veut empêcher la mutation

utilisateur.nom = 'Bob'; // Modification permise
utilisateur.couleur = 'bleu'; // Ignoré, ne peut pas ajouter de nouvelles propriétés
delete utilisateur.age; // Ignoré, ne peut pas supprimer de propriétés

console.log(utilisateur); // Attendu : { nom: 'Bob', age: 25 }
```

* **Object.preventExtensions()** :
Empêche l'ajout de nouvelles propriétés à un objet, mais permet la modification et la suppression des propriétés existantes.
## Exemple
```js
const livre = {
  titre: 'JavaScript: The Good Parts',
  auteur: 'Douglas Crockford'
};

Object.preventExtensions(livre); //bject.preventExtensions() prends en paramètre l'objet dont on veut empêcher la mutation

livre.titre = 'JavaScript: The Definitive Guide'; // Modification permise
livre.pages = 300; // Ignoré, ne peut pas ajouter de nouvelles propriétés
delete livre.auteur; // Suppression permise

console.log(livre); // Attendu : { titre: 'JavaScript: The Definitive Guide' }
```


## Exercice 1 : Utiliser Object.freeze()
Objectif : Créez un objet représentant un film et utilisez Object.freeze() pour empêcher toute modification.

## Exercice 2 : Utiliser Object.seal()
Objectif : Créez un objet représentant un utilisateur et utilisez Object.seal() pour empêcher l'ajout ou la suppression de propriétés, mais permettre la modification des propriétés existantes.