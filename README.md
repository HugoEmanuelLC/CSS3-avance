# CSS3-avance

### px, %, em, rem

- **em**

    * e « em » correspond à la taille de la police de caractère de l’élément en cours et si cette taille n’est pas redéfinie alors cette taille correspondra à la taille de la police de l’élément parent. Par exemple, si la taille de la police est définie à 20px alors 1em sera égale à 20px.

    * Cette unité pourra vous permettre de définir les marges intérieures « paddings » ou extérieures « margins » qui seront liées à la taille du texte et ainsi les redimensionner en fonction de cette dernière sur différents supports.

    * Ainsi sur un grand écran, les marges seront plus grandes tout comme la taille du texte et à l’inverse sur un petit écran (comme un écran de smartphone) les textes seront plus petits et les marges aussi.

    * Vous trouverez souvent les déclarations « margin: 1em » et « text-indent: 1.5em » en CSS.

- **rem**

    * L’unité « rem » signifiant « root em » reprend le principe de l’unité « em », c’est-à-dire correspondre à la taille de la police d’un élément et cet élément est l’élément racine du document (root).

    * Ainsi le « rem » permet de définir une valeur constante tout le long du document égale à la taille de la police de l’élément racine.

    * Cette unité peut être alors utilisée pour créer des éléments et propriétés CSS responsives puisque qu’elle s’adaptera à la taille de la police du support d’affichage.    

### < easing-function >

Le type de données CSS <easing-function> indique une fonction mathématique qui décrit la façon dont une valeur numérique évolue.

##### Syntaxe

Il existe trois types de fonctions de transition:

- linéaires
    * L'interpolation se fait à évolution constante, du début jusqu'à la fin. Ce mot-clé représente la fonction de transition décrite par cubic-bezier(0.0, 0.0, 1.0, 1.0).

- courbes de Bézier cubiques
    * cubic-bezier(x1, y1, x2, y2)

    * EASE , EASE-IN , EASE-IN-OUT , EASE-OUT

    * La notation fonctionnelle cubic-bezier() définit une courbe de Bézier cubique. Ces courbes étant continues, elles sont souvent utilisées afin de démarrer et de finir progressivement une interpolation. Elles sont parfois appelées fonctions de transition.

- en escalier
    La notation fonctionnelle steps() définit une fonction en escalier qui divise le domaine des valeurs de sorties en marches équidistantes.

    * steps(nombre_de_marches, direction)

    * jump-start indique une fonction continue à gauche : le premier saut a lieu au début de l'interpolation ;

    * jump-end indique une fonction continue à droite : le dernier saut a lieu à la fin de l'interpolation ;

    * jump-both indique une fonction continue à droite et à gauche avec des pauses au début et à la fin, ce qui se traduit par l'ajout d'une étape lors de l'itération de l'interpolation ;

    * jump-none indique qu'il n'y a pas de saut au début ou à la fin mais une temporisation de 1/n de la durée totale à chaque extrêmité.

    * start est équivalent à jump-start

    * end est équivalent à jump-end

    * end est la valeur par défaut.