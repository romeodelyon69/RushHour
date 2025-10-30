French :
Important : pour utiliser le notebook, il est essentiel de télécharger les fichiers d'initialisation GameP01.txt jusqu'à GameP40.txt et de référencer le chemin d'accès associé dans la variable file_path_rad au dans la première cellule du notebook. 

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

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
English : 
The associated project presents an algorithm capable of solving the Rush Hour puzzle. The goal is to move the red car out of the parking grid.
Each of the provided text files represents a different starting configuration to be solved.

The project is built around a main class called RushHourGame, which allows you to create a game instance and provides a set of methods to play and analyze the game.
Each instance includes a boolean isGraphic that determines whether or not to display the game visually, using the Pygame module for rendering.

Two solving algorithms are implemented:

The first one, bfs_search, performs a breadth-first search in the space of possible positions to find the fastest solution to the Rush Hour problem.

The second is similar but relies on a heuristic to explore positions more intelligently. Two heuristics are implemented:

The first is based on the number of cars blocking the red car.

The second penalizes these blocking cars even more if they themselves are blocked and cannot clear the path for the red car in a single move.

Finally, the project also includes a play() function that allows you to play a game manually (useful for debugging).
To play, simply select a car by its number (works for up to 9 cars) and move it using the corresponding arrow keys.
