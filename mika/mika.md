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


Permet aussi les calculs et opérations avec le placeholder : 

    var age = 10
    var capitaine = 50
    console.log(`Age du capitaine : $(age+capitaine)`);
    // Age du capitaine : 60
    
    console.log(`Avec 2 capitaines : $(2*(age+capitaine)`);
    // Avec 2 capitaines : 120
    
Ils s'utilisent aussi dans les fonctions : 

    function yo(){ return "--Flipidi flop Wesh 82--";}
    console.log(`La fonction old school : $(yo)} c'est sympa`;
    
Pour ajouter des accents graves dans votre placeholder : 

    var coucou = `\`Yo\` tout le monde c'est Hetic `;
    // "`Yo` tout le monde c'est Hetic "
    
### Gestion du multiligne

Plusieurs solutions existent pour faire du multilignes : 

- Antislash : 


        var coucou = "Salut \ 
        tout le monde";
    
- Addition : 

 

        var coucou = "Salut" + 
        " tout le monde";
        
        
- Retour à la ligne : 

 

        console.log(`Salut les héticiens et les
           héticiennes`);
           
        
