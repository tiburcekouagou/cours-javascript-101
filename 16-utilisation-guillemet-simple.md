```js
let myStr = "<a href=\"http://www.example.com\" target=\"_blank\">Link</a>";
```

Nous avons déjà parler d'échappement de caractères comme pour l'example ci-dessus. Vous placer un antislash `(\)` avant le guillemet puis JavaScript comprend que cela est supposé être littéralement un guillement dans la chaîne de caractère.

Cependant, cela ne veux pas dire que devez tout le temps échapper les caractères comment dans l'example ci-dessus. Il y a des manières bien plus simples d'avoir des guillemets dans une chaîne de caractères.

Une manière simple d'y parvenir est que, au lieu d'utiliser des guillemet-double `("")` pour déclarer les chaînes de caractères, utilisez des guillemets simples. Donc, une chaîne de caractère peut être entourrée par des guillemets simples ou doubles. Et voici à quoi ressemble l'example précédant quand on utilise des guillemets simples pour entourer la chaîne de caractère.

```js
let myStr = '<a href="http://www.example.com" target="_blank">Link</a>';
```

Et donc, on peut voir que c'est beaucoup plus simple, que le premier exemple. Et voilà ! 😀