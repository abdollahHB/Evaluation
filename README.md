# GestionStock TP

## Aperçu du Projet
Ce projet est une application Java conçue pour gérer les stocks et les commandes en utilisant Hibernate pour l'interaction avec la base de données. Il illustre les concepts clés de la mapping objet-relationnel (ORM) et de l'architecture orientée services.

### Fonctionnalités
- Gestion des catégories, produits et commandes
- Requêtes et affichage des données via Hibernate
- Tests des fonctionnalités avec des scénarios prédéfinis

## Structure du Projet
- `pom.xml`: Fichier de configuration Maven
- `src/main/java/ma/projet`:
  - `classes`: Classes d'entités représentant les tables de la base de données
  - `dao`: Interface d'accès aux données
  - `service`: Implémentation de la logique métier
  - `util`: Classes utilitaires pour la configuration Hibernate
  - `Main.java`: Point d'entrée de l'application
  - `Test.java`: Scénarios de test
- `src/main/resources`:
  - `hibernate.properties`: Configuration Hibernate

## Structure de la Base de Données
L'application interagit avec une base de données MySQL (`gestionstock`) contenant les tables suivantes :
- categorie
- commande
- lignecommandeproduit
- produit



## Résultats des Tests
L'application inclut des scénarios de test pour valider les fonctionnalités. Voici un exemple de sortie de test :

![Résultats des Tests](attachments/test_results.png)

## Instructions de Configuration
1. Clonez le dépôt
2. Configurez la connexion à la base de données dans `hibernate.properties`
3. Construisez le projet avec Maven :
   ```
   mvn clean install
   ```
4. Exécutez l'application :
   ```
   java -cp target/classes ma.projet.Main
   ```

## Utilisation
- Utilisez la classe `Test.java` pour exécuter les scénarios de test prédéfinis
- Modifiez les classes d'entités et les services pour étendre les fonctionnalités

## Licence
Ce projet est uniquement à des fins éducatives.