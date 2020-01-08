# Code créatif Module 02 couleur

## version
v 0.1.1

## objectif

Réaliser à l'aide du langage Processing les exercices suivants.
Un exercice est soit raté, soit réussit.
Chaque exercice rapporte des points, pour valider un module il faut obternir au moins 60% des points de l'ensemble du modules.
Dés que la norme n'est pas respectée, l'exercice est considéré comme raté.

L'ensemble des exercices sont à renvoyer par mail au correcteur en respectant l'arborescence et le nommage des dossiers, sous-dossiers et nom de fichiers. Si l'arborescence n'est pas respectée l'exercice ou le module ne seront pas corrigés et considérés comme ratés.
Vous avez des listes de `primitive, globale, opérateur, méthode, condition` ou `itération` que vous pourrez utiliser. Il n'est pas obligatoire de toutes les utiliser, par contre vous ne pouvez pas en utiliser d'autres.

La taille de la fenêtre pourra être changée par le correcteur.

Toutes les consignes sont valables pour l'ensemble du module sauf indication contraire.

```
dossier : nom prénom
sous-dossier : m##
sous-dossier : m##_ex##_nom
fichier :  m##_ex##_nom.pde
```

* exemple 

`Maurice_Dupont/m00/m00_ex_00_truc/m00_ex_00_truc.pde`


contraintes : 
respecter la [norme](https://github.com/StanLepunK/La-Voie-du-Code/blob/master/norme_voie_du_code.md)

## m02_ex00_rgb
```
sketch : m01_ex00_rgb.pde
intitulé :
Dans une fenêtre de 640 par 480.
À chaque clique de souris, la couleur de l'arrière plan changera.
À noter que la couleur va de 0 à 255.
```
```
primitive : float
globale : 
opérateur : =
méthode primaire : setup(), draw(), mousePressed()
méthode secondaire : size(), background(), random()
condition :
itération :
```

## m02_ex01_hsb
```
sketch : m01_ex01_hsb.pde
intitulé :
Dans une fenêtre de 640 par 480.
À chaque que la touche 'h' sera déclanchée la couleur de l'arrière plan changera.
À chaque que la touche 's' sera déclanchée la saturation de l'arrière plan changera.
À chaque que la touche 'b' sera déclanchée la luminosité de l'arrière plan changera.
```
```
primitive : float
globale : key, width, height, HSB
opérateur : = ==
méthode primaire : setup(), draw(), keyPressed()
méthode secondaire : size(), background(), random(), colorMode()
condition : if
itération :
```

## m02_ex02_set_pixel
```
sketch : m01_ex02_set_pixel.pde
intitulé :
Dans une fenêtre de 640 par 480.
attribué une couleur différente à chaque pixel.
```
```
primitive : int
globale : width, height
opérateur : = < ++ += +
méthode primaire : setup()
méthode secondaire : size(), set(), color(), random()
condition :
itération : while()
```

## m02_ex03_camaieu
```
sketch : m01_ex03_camaieu.pde
intitulé :
Créez une méthode camaieu().
Dans une fenêtre de 640 par 480.
Environement de couleur en HSB, 360, 100, 100.
Attribuez aux pixels un camaieu de couleur différent avec un gap de 25 autour d'une couleur que vous choisirez.
Vous définirez une valeur de votre choix pour la saturation et la luminosité.
Le camaieu devra être présent dès le début et devra changer à chaque clique de souris.
```
```
primitive : int, float
globale : width, height
opérateur : = < ++ += +
méthode primaire : setup(), draw(), mousePressed()
méthode secondaire : size(), set(), color(), colorMode(), random()
condition :
itération : while()
```
## m02_ex04_spectre
```
sketch : m01_ex04_spectre.pde
intitulé :
Créez une méthode spectre().
Dans une fenêtre de 640 par 480.
Environement de couleur en HSB, 360, 100, 100.
créer un spectre de couleur spécifique à une couleur, en haut à gauche on trouvera la couleur pure, en haut à droite la couleur désaturée, donc blanc et plus nous descendrons plus la couleur sera sombre. Donc sur la gauche cela ira de la couleur au noir tandis que sur la droite cela ira du blanc au noir.
Le spectre devra être présent dès le début et devra changer de couleur à chaque clique de souris.
```
```
primitive : int, float
globale : width, height, g.colorModeX
opérateur : = < > - += +
méthode primaire : setup(), draw(), mousePressed()
méthode secondaire : size(), set(), color(), colorMode(), random(), map()
condition :
itération : while()
```

## m02_ex05_disque
```
sketch : m01_ex05_disque.pde
intitulé :
Créez une méthode disque().
Dans une fenêtre de 640 par 480.
Environement de couleur en HSB, 360, 100, 100.
Créer un disque donc chaque rayon partiront du centre de la fenêtre et seront d'une couleur différente sur fond noir.
Le disque devra appraitre dés le début et changer de couleur, de taille et de nombre de traits à chaque clique de souris.
```
```
primitive : int, float
globale : width, height, g.colorModeX, PI
opérateur : = < > - += + ++ / 
méthode primaire : setup(), draw(), mousePressed()
méthode secondaire : size(), set(), color(), colorMode(), random(), map(), int(), sin(), cos(), background().
condition :
itération : while()
```

## m02_ex06_chose
```
sketch : m01_ex06_chose.pde
intitulé :
Créez une méthode chose().
Dans une fenêtre de 640 par 480.
Environement de couleur en HSB, 360, 100, 100.
Créer une forme donc chaque trait partira du centre et varira de rayon de façon hasardeuse et harmonique. 
La couleur parcourera le spectre de couleur petit à petit.
La chose devra appraitre dés le début et changer de couleur, de taille et de nombre de traits à chaque clique de souris.
```
```
primitive : int, float
globale : width, height, PI
opérateur : = < - += + ++ * /
méthode primaire : setup(), draw(), mousePressed()
méthode secondaire : size(), set(), color(), colorMode(), random(), map(), noise(), int(), sin(), cos(), background().
condition :
itération : while()
```

## m02_ex07_soleil
```
sketch : m01_ex07_soleil.pde
intitulé :
Créez une méthode soleil().
Dans une fenêtre de 640 par 480.
Environement de couleur en HSB, 360, 100, 100.
Créer une forme dont la forme rapellera celle d'un soleil.
Chaque trait partira du centre et sa logueur variara de façon sinusoidale. 
La couleur varira en camaieu autour d'une couleur que vous aurez choisit.
Le Centre du soleil sera blanc pour atteindre sa saturation maximum à son extrémité.
La Soleil devra appraitre dés le début et changer de couleur, de taille, de forme et son nombre de traits à chaque clique de souris.
```
```
primitive : int, float
globale : width, height, PI
opérateur : = < - += + * /
méthode primaire : setup(), draw(), mousePressed()
méthode secondaire : size(), set(), color(), colorMode(), random(), map(), noise(), int(), sin(), cos(), abs(), background().
condition :
itération : while()
```



