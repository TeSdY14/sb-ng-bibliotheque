# sb-ng-bibliotheque
Application d'administration de bibliothèque réalisée avec Java Spring Boot 2 et Angular 7

## Expression du Besoin 
### User Stories
#### En tant qu'Administrateur de la bibliothèque je dois pouvoir 
- Ajouter un nouveau livre, 
- Rechercher un livre grâce à son [ISBN](https://fr.wikipedia.org/wiki/International_Standard_Book_Number) ou grâce à tout ou partie de son titre, ceci afin de visualiser l'ensemble des informations,
- Suite à une recherche de livre(s), modifier ou supprimer chacun des livres dans la liste qui s'affiche, 
- Ajouter un nouveau client, 
- Recherche un client grâce à son email ou tout ou partie de son nom de famille, afin de visualiser l'ensemble de ses informations;
- Suite à une recherche de client(s), modifier ou supprimer chacun des clients dans la liste qui s'affiche
- Ajouter un nouvel emprunt, celui ci est lié entre le livre sorti et l'emprunteur,
- Recherche la liste des emprunts d'un client grâce à son email et la liste des emprunts réalisés jusqu'a une certaine date : voir l'historique
- Suite à une recherche d'emprunts, modifier ou clôturer chacune des emprunts dans la liste qui s'affiche, 
- Avoir sur l'application, un menu général qui permet d'accéder à la page de gestion des livres, celle des clients et celles des emprunts; afin d'être le plus efficace dans l'utilisation de l'application. 

_(pas de gestion de sécurité : "identification", dans cette première version)_ 


## Apercu UML 
### Entités pertinentes
Livre (Book) ;
Catégorie de livre (Category) ;
Client (Customer) ;
Emprunt (Loan) ;
Bibliothèque (Library) . 

### Liaisons
- Un Livre appartient à une et une seule catégorie ;
- Une Catégorie peut avoir zero ou plusieurs livre(s) ;
- Un Client peut effectuer zéro ou plusieurs emprunts de livre(s) ; 
- Un Livre ayant plusieurs exemplaires, il peut etre emprunté par zéro ou plusieurs Client(s) ; << Cette relation génère une association :  
    - Un Emprunt a une date de début et de fin : Association porteuse de propriétés ! 

![image](https://drive.google.com/uc?export=view&id=1qAtrovFkgDo9okVJBYTkrGSnBuSyO3hu)






