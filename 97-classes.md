## Les classes

une classe est une structure qui permet de définir des objets en utilisant une syntaxe plus proche de la programmation orientée objet (POO) traditionnelle. Les classes permettent de définir des objets avec des propriétés et des méthodes spécifiques.  
### Syntaxe de Base d'une Classe
Voici un exemple simple de déclaration d'une classe en JavaScript :  
```js
class Animal {
    constructor(nom, age) {
        this.nom = nom;
        this.age = age;
    }

    direBonjour() {
        console.log(`Bonjour, je m'appelle ${this.nom} et j'ai ${this.age} ans.`);
    }
}
```
Dans cet exemple, `Animal` est une classe qui définit des objets représentant des animaux. La classe a un **constructeur** pour initialiser les propriétés `nom` et `age`, ainsi qu'une méthode `direBonjour` pour afficher un message de salutation.  
**Un constructeur** est une méthode spéciale d'une classe qui est automatiquement appelée lorsqu'une instance de la classe est créée. Son rôle principal est d'initialiser les propriétés de l'objet nouvellement créé.  
Le constructeur est défini à l'intérieur de la classe à l'aide de la méthode spéciale `constructor`