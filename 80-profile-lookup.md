# 80 - Recherche de profile
Nous disposons d'un ensemble d'objets représentant différentes personnes dans nos listes de contacts.
Une fonction lookUpProfile qui prend name et une propriété ( prop) comme arguments a été pré-écrite pour vous.
La fonction doit vérifier s'il name s'agit d'un contact réel firstName et que la propriété donnée ( prop) est une propriété de ce contact.
Si les deux sont vrais, renvoyez la « valeur » de cette propriété.
Si namene correspond à aucun contact, renvoyez la chaîne No such contact.
Si propne correspond à aucune propriété valide d'un contact trouvé, namerenvoyez la chaîne No such property.

## Exemple 1:
Nous allons commencer à `i = 10` et boucler while `i > 0`. Nous allons décrémenter `i` de `2` chaque boucle avec `i -= 2`.

```js
        const contacts = [
        {
            firstName: "Akira",
            lastName: "Laine",
            number: "0543236543",
            likes: ["Pizza", "Coding", "Brownie Points"],
        },
        {
            firstName: "Harry",
            lastName: "Potter",
            number: "0994372684",
            likes: ["Hogwarts", "Magic", "Hagrid"],
        },
        {
            firstName: "Sherlock",
            lastName: "Holmes",
            number: "0487345643",
            likes: ["Intriguing Cases", "Violin"],
        },
        {
            firstName: "Kristian",
            lastName: "Vos",
            number: "unknown",
            likes: ["JavaScript", "Gaming", "Foxes"],
        },
        ];

        function lookUpProfile(name, prop) {

        //  ...
        }

        lookUpProfile("Akira", "likes");
```
`lookUpProfile("Kristian", "lastName")` devrait renvoyer la chaîne `Vos`
`lookUpProfile("Sherlock", "likes")` devrait renvoyer `["Intriguing Cases", "Violin"]`
`lookUpProfile("Harry", "likes")` devrait renvoyer un tableau
`lookUpProfile("Bob", "number")` devrait renvoyer la chaîne `No such contact`
`lookUpProfile("Bob", "potato")` devrait renvoyer la chaîne `No such contact`
`lookUpProfile("Akira", "address")` devrait renvoyer la chaîne `No such property` 


## SOLUTION

```js
        const contacts = [
        {
            firstName: "Akira",
            lastName: "Laine",
            number: "0543236543",
            likes: ["Pizza", "Coding", "Brownie Points"],
        },
        {
            firstName: "Harry",
            lastName: "Potter",
            number: "0994372684",
            likes: ["Hogwarts", "Magic", "Hagrid"],
        },
        {
            firstName: "Sherlock",
            lastName: "Holmes",
            number: "0487345643",
            likes: ["Intriguing Cases", "Violin"],
        },
        {
            firstName: "Kristian",
            lastName: "Vos",
            number: "unknown",
            likes: ["JavaScript", "Gaming", "Foxes"],
        },
        ];

        function lookUpProfile(name, prop) {

        for (let i = 0; i < contacts.length; i++){
            if (contacts[i].firstName == name ){
                if (contacts[i].hasOwnProperty(prop)){
                    return contacts[i][prop];
                }
                else{
                    return "No such property";
                }
            }
        }
            return "No such contact"
        }
```