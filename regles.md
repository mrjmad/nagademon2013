# Règles de déroulement d'une partie


## Phases d'une partie

Une partie se découpe en round. Un round se divise en tour de jeu. Il y a autant de tour de jeu par round que de joueur. Lors de son tour, un joueur peut effectuer 3 actions plus deux actions d'appel de robot. Les actions d'appel de robot permettent de téléporter un robot du garage de l'équipe sur l'un des plots entourant le commandeur porte drapeau de l'équipe. Cette action n'a de sens que tant que l'équipe n'est pas totalement sur le terrain.

Les trois actions qui restent peuvent servir à deux choses : 

* gérer les déplacements et les attaques d'un robot
* appeler un robot

Lorsque le joueur décide d'utiliser une action pour faire agir un robot il peut à la fois faire se déplacer et faire attaquer le robot en question. Une action ne peut pas être découper en plusieurs parties qui seraient exécutées en plusieurs fois. 

Prenons un exemple : 

Alice et Bruno jouent ensemble, c'est au tour d'Alice de jouer. Elle a 3 robots présent sur le plateau de jeu R1, R2 et R3. Bruno lui a deux robots T1 et T2. Alice peut décider de commencer à faire agir R1, lui faire faire 2 déplacement, lui faire tirer sur T1 puis lui faire encore traverser un pont. 
Par contre, elle ne peut pas commencer à faire se déplacer R1, lui faire faire deux déplacement et tirer sur T1, puis décider de faire tirer R2 sur T1 puis de revenir à R1 pour lui faire finir son déplacement.


## Déplacement sur le terrain de jeu

Un robot doit toujours finir un déplacement sur un plot. Il est pas possible de rester
sur un pont. Il ne peut y avoir plusieurs robots sur le même plot. Un robot ne peut donc
pas finir son déplacement sur un plot qui serait déjà occupé par un autre robot. Lorsqu'un robot présent sur un plot est détruit, le plot sur lequel il se trouvait est à nouveau considéré comme vide.

Chaque robot a une vitesse en nombre de ponts par tour. Un robot peut se déplacer de tout ou parti de sa vitesse. Par exemple si un robot peut parcourir 3 ponts par tour, il peut très bien décider de n'en traverser qu'un.

Un robot peut interrompre son déplacement pour effectuer une action pour le poursuivre. Par exemple un robot qui a pour vitesse 3 ponts par tour, peu se déplacer de deux ponts puis tirer sur un autre robot puis traverser un dernier pont pour se rendre sur un nouveau plot.

## Combats

### Armes
Chaque arme possède trois caractéristiques : 

* sa fréquence de tir par tour
* sa portée de tir
* ses dégats

Une arme qui a 2 comme fréquence de tir par tour pourra donc être utilisée deux fois dans le même tour, sur deux cible potentiellement différentes. Un robot peut commencer un déplacement tirer une première fois, continuer son déplacement et tirer u ne nouvelle fois avec la même arme, sur une nouvelle cible (à condition que l'arme est une fréquence de tir de 2, bien entendu. 

### Dégâts et Blindage

Chaque robot possède un certain nombre de point de structure. Lorsqu’il n'a plus de points de structures, il est détruit. Un robot peut également être protégé par du blindage. A chaque fois qu'un robots subira des dégâts, il devra soustraire de ses points de structures les dégâts reçus moins son total de blindage. La formule de calcul des dégâts réels est donc : Dégâts réels = Dégâts reçus - Blindage.


##Fin de partie

Il y a deux manières de finir une partie : 

* le commandeur porte drapeau d'une des deux équipes est détruit. Dans ce cas, c'est l'équipe qui possède encore son commandeur qui gagne.
* Le vingt-cinquième round vient de se terminer. L'équipe qui possède le plus de robots en fonctionnement est déclarée gagnante. Si aucune équipe n'a perdu de robot, les deux équipes ont perdus. Si les deux équipes ont perdus autant de robots l'une que l'autre, c'est celle qui a eu le moins de robots blessés qui est déclaré gagnante. Si les deux équipes ont perdu le même nombre de robots et ont autant de robots blessés l'une que l'autre, les deux équipes sont déclarées perdantes.


