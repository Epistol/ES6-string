# ES6 Template String


Source : https://developers.google.com/web/updates/2015/01/ES6-Template-Strings 


## Historique

Les chaînes de caractères ont été historiquement limité en terme de compatibilité. ES6 Template Strings à changé la façon de définir les caractères avec une meilleure :

1. Interpolation
2. Expressions imbriquées
3. Multilignes
4. Formatting
5. HTML echappé sécurisé


### Syntaxe

Template strings utilise l'accent grave (altgr+7) plutot que des simples : " ' . 

    var salut = `Hetic World`;

### Substitution de chaînes de caractères

Template Strings peut utiliser des espaces réservés (placeholder)  en utilisant ${} comme syntaxe :

    var nom = `Brontis`;
    console.log(`Salut ${nom} !`);

    // => "Salut, Brontis ! "


