Le projet associé présente un algorithme capable de résoudre le jeu du RushHour. L'objectif étant de faire sortir la voiture rouge du parking.  
Les fichiers textes associés representent chacun  une position de départ qu'il faut résoudre. 

Le projet est constitué d'une classe principale RushHourGame, qui permet de créer une partie et qui contient un ensemble de méthode pour jouer et analyser le jeu.
Chaque instance est muni d'un booléen isGraphic qui permet de choisir si l'on souhaite ou non afficher la partie en cours, affichage réaliser à l'aide du module Pygame. 

Deux algos de résolutions sont ensuite proposé, le premier bfs_search effectue un parcourt en largeur dans l'espace des positions possibles afin de trouver la 
solution rapide au problème du RushHour. 
Le deuxième est relativement similaire mais se base sur une heuristique pour explorer les positions plus intelligement. 
Deux heuristiques sont implementées, une première qui se base sur le nombre de voiture bloquant la voiture rouge. La seconde pénalise d'autant plus fortement ces 
voitures bloquantes si elles même sont également bloquées et ne peuvent pas libérer le passage à la voiture rouge en 1 seul coup. 

Enfin, le projet contient également une fonction play(), qui permet de lancer une partie à laquelle le joueur pourra jouer (utile pour déboguer). Pour jouer, il suffit de sélectionner la voiture par son numéro (fonctionne jusqu'à 9 voitures) et de la déplacer avec les flèches associées. 
