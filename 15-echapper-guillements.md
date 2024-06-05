## Echapper les guillemets  
Pour inclure des guillemets dans une chaîne de caractères délimitée par des guillemets du même type, vous devez les "échapper" en les précédant d'un backslash (\). Par exemple :  
````js
let message = "Il a dit : \"Bonjour, monde !\"";
console.log(message); // Affiche "Il a dit : "Bonjour, monde !""
````  
Dans cet exemple, les guillemets doubles à l'intérieur de la chaîne sont échappés pour éviter de les confondre avec les guillemets délimitant la chaîne.
De même, si vous utilisez des guillemets simples pour délimiter la chaîne, vous devez échapper les guillemets simples à l'intérieur de la chaîne :  
````js
let message = 'Il a dit : \'Bonjour, monde !\'';
console.log(message); // Affiche "Il a dit : 'Bonjour, monde !'"
````
En échappant les guillemets, vous pouvez les inclure dans votre chaîne de caractères sans provoquer d'erreur de syntaxe.