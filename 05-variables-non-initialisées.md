## Variables Non Initialisée 
 En JavaScript, si vous déclarez une variable sans l'initialiser explicitement avec une valeur, elle prendra automatiquement la valeur **undefined**. Par exemple :  
 ````js
 let x;
 console.log(x); // Affiche undefined
 ````  
 Dans cet exemple, la variable x est déclarée mais n'est pas initialisée avec une valeur spécifique, donc elle est automatiquement initialisée à **undefined**.Il est important de noter que undefined est une valeur spéciale en JavaScript qui est utilisée pour représenter l'absence de valeur.  
 ## Casse des variables
  les variables sont sensibles à la casse, ce qui signifie que les majuscules et les minuscules sont distinguées. Cela signifie que maVariable, MaVariable et MAVARIABLE sont considérées comme trois variables distinctes. Par exemple :  
  ````js
  let maVariable = 10;
let MaVariable = 20;

console.log(maVariable); // Affiche 10
console.log(MaVariable); // Affiche 20
  ````  
Il est important de faire attention à la casse lorsque vous utilisez des variables dans votre code JavaScript, car une erreur de casse peut entraîner des erreurs ou des résultats inattendus.  