
# TP Guidé en Kotlin : Gestion des salles avec les collections

## Objectif

L'objectif de ce TP est de guider les étudiants à travers les étapes de création d'un système de gestion des salles en utilisant Kotlin. À la fin de ce TP, vous aurez implémenté des opérations CRUD (Create, Read, Update, Delete) pour gérer des objets Salle.

**Prérequis**

-   Connaissance de base en programmation orientée objet.
-   Connaissance de base en Kotlin (classes, interfaces, collections).

## Énoncé du TP

### Partie 1 : Couche Métier

1.  Créez une classe Salle avec les propriétés suivantes :

-   **id** (entier, auto-incrémenté)
-   **code** (chaîne de caractères)
-   **libelle** (chaîne de caractères)

3.  Ajoutez un constructeur qui permet d'initialiser code et libelle. L'id doit être auto-incrémenté.
4.  Implémentez des accesseurs pour les propriétés. En Kotlin, cela est souvent fait via des propriétés avec var ou val.
5.  Définissez une méthode toString() pour afficher les détails d'une salle.

### Partie 2 : Couche Accès aux Données

1.  Créez une interface générique **IDao<T>** avec les méthodes suivantes :

-   create(o: T): Boolean
-   delete(o: T): Boolean
-   update(o: T): Boolean
-   findById(id: Int): T?
-   findAll(): List<T>

3.  Implémentez cette interface dans une classe SalleService. Utilisez une List pour stocker les salles.

### Partie 3 : Couche de Présentation

-   Dans une fonction **main**, créez et manipulez plusieurs instances de Salle.

-   Ajoutez des salles.
-   Affichez toutes les salles.
-   Supprimez une salle.
-   Modifiez et mettez à jour une salle.
-   Affichez de nouveau toutes les salles.
