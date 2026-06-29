# JustStreamIt - Interface Utilisateur d'une Application Web

JustStreamIt est une application web de streaming (VOD) qui permet de visualiser en temps réel les classements des meilleurs films, catégories spécifiques et détails de films grâce à une intégration dynamique de données provenant d'une API locale (OCMovies-API).

Ce projet a été réalisé dans le cadre de la formation Développeur d'Application JavaScript / Intégrateur Web d'OpenClassrooms.

---

## 📱 Fonctionnalités

* **Sélection du Meilleur Film :** Affichage dynamique du film le mieux noté toutes catégories confondues avec son résumé.
* **Grilles Dynamiques par Catégorie :** Visualisation des films les mieux notés, d'une catégorie fixe (Action, Sci-Fi) et de catégories personnalisables par l'utilisateur via un menu déroulant.
* **Modale de Détails Complète :** Ouverture d'une fenêtre modale au clic sur un film affichant toutes les informations détaillées (acteurs, réalisateurs, box-office, description longue...) conformément aux maquettes Desktop, Tablette et Mobile.
* **Design 100% Responsive :** Interface optimisée pour s'adapter parfaitement aux écrans d'ordinateurs, de tablettes et de smartphones.

---

## 🛠️ Prérequis

Pour faire fonctionner ce projet sur votre machine, vous devez avoir installé :
* **Python 3.x**
* **Git**
* Un navigateur web moderne (Chrome, Firefox, Edge, etc.)

---

## 🚀 Installation et Lancement

### 1. Cloner et lancer l'API Locale (Backend)

L'application frontend dépend de cette API pour récupérer les données des films. Suivez ces étapes pour la lancer :

1. Ouvrez un terminal et clonez le dépôt de l'API :
    ```bash
   git clone [https://github.com/OpenClassrooms-Student-Center/OCMovies-API-EN-FR.git](https://github.com/OpenClassrooms-Student-Center/OCMovies-API-EN-FR.git)

    ```bash
   cd ocmovies-api-fr
    ```bash
### 2. Créez un environnement virtuel
    ```bash
Windows : python -m venv env
    ```bash
Mac/Linux : python3 -m venv env
    ```bash
### 3. Activez un environnement virtuel
    ```bash
Windows : env\Scripts\activate
    ```bash
Mac/Linux : source env/bin/activate
    ```bash
### 4. Installez les dépendances requises
    ```bash
pip install -r requirements.txt
    ```bash
### 5. Initialisez et alimentez la base de données (uniquement au premier lancement)
    ```bash
python manage.py create_db
    ```bash
### 6. Démarrez le serveur local
    ```bash
    python manage.py runserver