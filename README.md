# Gestion des Services et Employés avec JSF, XAMPP et NetBeans

Ce projet est une application web Java basée sur JSF qui permet la gestion des services et des employés d'une entreprise. Il utilise XAMPP comme serveur local pour la base de données MySQL et NetBeans comme environnement de développement intégré.

# Configuration requise

XAMPP : Télécharger XAMPP
NetBeans : Télécharger NetBeans

# Configuration de la base de données

Installez XAMPP sur votre machine.
Lancez XAMPP et démarrez les services Apache et MySQL.
Accédez à phpMyAdmin (http://localhost/phpmyadmin/) et créez une nouvelle base de données nommée gestion_employes.
Importez le fichier database.sql situé dans le répertoire database pour créer les tables nécessaires.

# Configuration du projet dans NetBeans

Ouvrez NetBeans et importez le projet.
Assurez-vous que le serveur GlassFish est configuré dans NetBeans.
Modifiez le fichier persistence.xml dans le répertoire src/META-INF pour correspondre à vos paramètres de base de données.
xml
Copy code
<persistence-unit name="GestionEmployesPU" transaction-type="JTA">
    <jta-data-source>jdbc/gestion_employes</jta-data-source>
    <properties>
        <!-- Configurations de la base de données -->
        <property name="javax.persistence.schema-generation.database.action" value="update" />
    </properties>
</persistence-unit>

# Exécution de l'application

Déployez l'application sur le serveur GlassFish depuis NetBeans.
Accédez à l'application à l'adresse http://localhost:8080/NomDuProjet/.

# Fonctionnalités

Gestion des Services :
Ajout, suppression et modification des services.

# AJOUT 

![ajouterservice](https://github.com/ouarriorxx/JSF/assets/143946046/088d3286-443e-41fe-8570-3b569c5907a9)

# SUPPRESSION

![supprimerservice1](https://github.com/ouarriorxx/JSF/assets/143946046/05372a20-50a3-4efa-8ce7-d3669d226830)
![supprimerservice2](https://github.com/ouarriorxx/JSF/assets/143946046/9143cf3c-b89e-469d-aa3c-ea6644cfba67)

# MODIFICATION

![modifierservice](https://github.com/ouarriorxx/JSF/assets/143946046/48e30604-50ae-4508-a9e3-8a85eebddd07)


Gestion des Employés :
Ajout, suppression et modification des employés.

# AJOUT

![ajouteremployee](https://github.com/ouarriorxx/JSF/assets/143946046/5b845e9f-e406-4e3e-b075-33e9fd529b6a)

# SUPPRESSION

![supprimeremployee](https://github.com/ouarriorxx/JSF/assets/143946046/167001ea-0a27-4133-b962-60eceb67f2a2)

# MODIFICATION

![modifieremployee](https://github.com/ouarriorxx/JSF/assets/143946046/9d678294-3bc1-4dbd-9bf2-b732c554a41d)



Association des employés à des services.
Affichage détaillé :
Affichage des informations détaillées sur les employés.
Structure du Projet
Expliquez brièvement la structure des répertoires du projet.

sql
Copy code
/
|-- src/            # Code source de l'application
|-- WebContent/    # Ressources web (pages JSF, CSS, etc.)
|-- database/      # Script SQL pour la création de la base de données
|-- ...

# Contributeur
OUARARI kawtar 
