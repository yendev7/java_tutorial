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


# L'heritage (Extends)
    Si une classe B herite d'une classe A cela veut dire que la classe B est la classe A car il elle herite de toutes les propiétés de la classe A.

# L'aggregation 
    -   le membre fait partie de l'objet
    -   le membre peut appartenir a plusieurs objets a la fois;
    -   la creation du membre n'est pas géré par l'objet

# Super()
    - utilisé pour appelé le contructeur du parent direct. 

# Bloc d'initialisation
    - # Static : on le fait dans un accolade
        ** initialisation des variable : ex: static nomVarible
    -   Le bloc d'initialisation d'instance est utilisé pour initialiser les membres de l'instance (les propriétés de l'objet). Il s'execute a chaque qu'un objet est créé.

    les 3 regles pour linitialisation d'instance: 
        - Le bloc d'initialisation d'instance est cré quand l'instance est créé
        - Ce bloc est invoqué apres que le constructeur de la super classe est invoqué
        - Ce bloc vient dans l'ordre dans lequel il apparait.

    - # Instance: ex:         class A {
                                         
                            }

# Les modificateurs d'acces 
C'est mot clé qui definit l'accessibilité et la portée d'une methode ou d'une classe....

                Classe       Package      Sous-classe      Globale
                                    
Private            v             x            x                 x   

Default            v             v            x                 x

Protected          v             v            v                 x

Public             v             v            v                 v

# Pour les classes il faut les mettre en public ou en defaut mais pour les champs il faut toujours les mettre en private et y avoir acces via les seters et geters

# Classe abstraite
    L'abstraction de données est le processus consistant à masquer certains détails et à ne montrer que les informations essentielles à l'utilisateur. Elle se fait au moyen d'une interface ou une classe abstraite.
        -   On declare une classe abstracte avec le mot cle Abbstract.
        -   Une classe abstract peut avoir des methodes non abstraite.
        -   Une classe abstraite est non instanciable.
        -   Une classe abstraite peut avoir des methodes finales.
        -   Une classe abstraite peut aussi avoir le methode statique et un constructeur

    Une interface est represente le template ou le plan que doir suivre une classe      
        # Déclarattion: interface NomInterface (toujours respecter le PascalCase)
        -Une interface ne contient que des methodes abstraites