But : pouvoir afficher mon CV, au choix, sous forme :
  - r�sum�e
  - d�taill�e
� partir d'une m�me table lue en base de donn�es
sur ma ge personnelle free.

Au d�part je voulais le faire avec symfony 2 mais je me suis heurt� � 2 types de contraintes :
1) Le tutoriel dans openclassrooms n'est pas en phase avec la version de symfony que j'ai pu charger => pour le moment je n'arrive pas � cr�er de bundle utilisable
2) Le site de free est en train de migrer vers la version 5 de PHP (au lieu de 4) mais le serveur sur lequel 
se trouve ma page personnelle est en PHP 5.1 apr�s migration et il fallait au moins la version 5.2 pour Symfony 2

Enfin je n'ai pas pu me connecter avec PDO sur ma base MySql car cette fois c'est le serveur MySql de free qui refus (alors que l'acc�s avec PDO fonctionnait tr�s bien en local avec PHP 5.6 sur XAMPP)

C'et pourquoi, finalement, j'ai cr�� une page PHP toute simple pour lire le CV d�taill�, puis je l'ai dupliqu�e en changeant la requ�te SQL afin d'obtenir la version r�sum�e
Puis j'ai cr�� une page HTML b�te � en pleurer qui permet de choisir entre ces 2 pages PHP.

Conclusion : cela fonctionne, m�me sur ma page free....