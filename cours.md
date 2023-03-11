# Finale : C'est une constante, on ne peut plus lui changer de valeur apres l'avoir initialisée
    - Methode 

    - Classe : Final devant une classe, veut dire qu'elle ne peut pas etre heritée

class Person {
    Private String name;
    final private int age = 25;
}


  # nb: final sur methode, dit a la methode que cest sa version finale donc ne peutplus changer de valeu, Donc overinding impossible.

  # Overloading 
    - est utilisé pour augmenter la visibilite d'un programme. 
    - Il se fait à l'interieur de la meme classe. 
    - Les parametres doivent etre differents (types et nombres).
    - Ne peut etre effectue en modifiant uniquement le type de retour de la methode. Le type de retour peut etre identique ou different, mais vous devez changer les parametres. 

  # Overrinding 
    - est utilisé opur fournir l'implementattion specifique d'ue methode qui est deja fourni par la superclasse(classe parent). 
    - Il se fait dans deux classe qui ont une relation d'heritage. 
    - Les parametres doivent etre les memes (types et nombres).
    - Le type de retour doit etre identique et covariant (doit toujours garder la structure de l'autre).
