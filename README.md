# Mon vieux Grimoire

Ce dépôt contient le backend de l'application Mon Vieux Grimoire : un site web de référencement et de notation de livres.


## Contexte
Je suis développeur back-end en freelance depuis maintenant un an dans la région de Lille. J'ai l’habitude de travailler avec Kévin, un développeur front-end plus expérimenté que moi, et qui a déjà un bon réseau de contacts dans le milieu.  
Kévin me contacte pour me proposer de travailler avec lui en mutualisant nos compétences front / back sur un tout nouveau projet qui lui a été proposé. Il s’agit d’une petite chaîne de librairies qui souhaite ouvrir un site de référencement et de notation de livres.  

## Prérequis
Avant d'installer et d'exécuter ce projet, assurez-vous d'avoir installé :

-   Node.js (version v20.2.0)
-   npm (version 9.6.6)

## Installation

Suivez les étapes ci-dessous pour installer et configurer le projet localement :
1. Clonez ce dépôt sur votre machine :\
   `git clone https://github.com/yasminedevv/openclassroom_projet06`
2. Accédez au répertoire du projet :\
   `cd Projet_06-Backend
3. Installez les dépendances nécessaires avec la commande suivante :\
   `npm install`

## Configuration de la Base de Données
Avant de lancer le projet, assurez-vous d'avoir configuré votre base de données MongoDB. Vous pouvez suivre les étapes suivantes :
1. Accédez au site web de MongoDB https://www.mongodb.com/cloud/atlas/register et inscrivez-vous pour obtenir un compte.
2. Une fois que vous avez accès à votre tableau de bord, créez un cluster et configurez-le selon vos besoins.
3. Récupérez votre code URI sur MongoDB et ajoutez-le dans un fichier .env que vous créez à la racine du projet. Configurez les variables d'environnement suivantes (variables listées dans le fichier .env):

## Sécurité
- Le mot de passe de l'utilisateur doit être haché.
- L'authentification doit être renforcée sur toutes les routes livre (book) requises.
- Les adresses électroniques dans la base de données sont uniques, et un plugin Mongoose approprié est utilisé pour garantir leur unicité et signaler les erreurs.
- La sécurité de la base de données MongoDB (à partir d'un service tel que MongoDB Atlas) ne doit pas empêcher l'application de se lancer sur la machine d'un utilisateur.
- Les erreurs issues de la base de données doivent être remontées.

## Fonctionnalités :
Gestion des livres : ajout, mise à jour et suppression de livres.\
Notation des livres : possibilité de noter les livres sur une échelle de 0 à 5.\
Authentification : inscription et connexion des utilisateurs.