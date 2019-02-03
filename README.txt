But : pouvoir afficher mon CV, au choix, sous forme :
  - résumée
  - détaillée
à partir d'une même table lue en base de données
sur ma ge personnelle free.

Au départ je voulais le faire avec symfony 2 mais je me suis heurté à 2 types de contraintes :
1) Le tutoriel dans openclassrooms n'est pas en phase avec la version de symfony que j'ai pu charger => pour le moment je n'arrive pas à créer de bundle utilisable
2) Le site de free est en train de migrer vers la version 5 de PHP (au lieu de 4) mais le serveur sur lequel 
se trouve ma page personnelle est en PHP 5.1 après migration et il fallait au moins la version 5.2 pour Symfony 2

Enfin je n'ai pas pu me connecter avec PDO sur ma base MySql car cette fois c'est le serveur MySql de free qui refus (alors que l'accès avec PDO fonctionnait très bien en local avec PHP 5.6 sur XAMPP)

C'et pourquoi, finalement, j'ai créé une page PHP toute simple pour lire le CV détaillé, puis je l'ai dupliquée en changeant la requête SQL afin d'obtenir la version résumée
Puis j'ai créé une page HTML bête à en pleurer qui permet de choisir entre ces 2 pages PHP.

Conclusion : cela fonctionne, même sur ma page free....