Movie.where(already_seen:true)
2.1. Exo 1 : Allociné

c) Un peu de freestyle
Crée une entrée avec un film de ton choix (un film que tu as déjà vu). Je veux juste que l'ensemble des attributs soient renseignés.
reponse
Movie.create(name:"the game", year:2015, genre:"action", synopsis:"text", director:"mohamed", allocine_rating:4.7,
my_rating:5, already_seen:true)


Modifie la note Allociné de Beowulf pour qu'elle soit à 4,7. Ce chef-d’œuvre mérite d'être reconnu comme tel.
reponse
Movie.where(name:"beowulf").update(allocine_rate:4.7)


Modifie le genre de l'Exorciste pour que ça soit une comédie. Avec un peu de chance ta petite soeur va tomber dessus.
reponse
Movie.where(name:"l'exorciste").update(genre:comedie)


Affiche, avec une commande en Movie.where, l'ensemble des films que tu as déjà vus.
reponse
Movie.where(already_see:true)



À partir de cet array de films que tu as déjà vus, supprime le premier de ta BDD.
reponse
Movie.where(already_see:true).delete

