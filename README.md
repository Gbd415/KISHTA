KISHTA – Application de gestion de paie pour PME/PMI
====================================================

Présentation
------------
Kishta est une application web développée avec Django et Bootstrap, destinée à automatiser la gestion de la paie au sein des petites et moyennes entreprises. Elle permet aux administrateurs de gérer les employés, les départements, les postes et les bulletins de paie, tandis que les employés peuvent consulter et télécharger leurs bulletins en PDF.

Fonctionnalités principales
---------------------------
- Authentification sécurisée (Admin / Employé)
- Gestion des employés (matricule, salaire, poste, département)
- Gestion des départements et des postes
- Création de bulletins de paie avec :
  - Salaire de base
  - Primes
  - Retenues
  - Calcul automatique du net à payer
  - Génération du PDF avec logo et en-tête
- Consultation et téléchargement des bulletins
- Interface responsive et professionnelle

Technologies utilisées
----------------------
- Backend : Django (Python)
- Frontend : HTML, CSS, Bootstrap
- Base de données : SQLite (par défaut Django)
- PDF : WeasyPrint
- Contrôle de version : GitHub

Installation
------------
1. Cloner le dépôt :
   git clone https://github.com/ton-utilisateur/KISHTA.git

2. Décompresser Gestion de Paie_KISHTA
   entrer dans le cmd ou powershell:
   cd kishta
   cd kishta
   source env/bin/activate  (Linux/macOS)
   env\Scripts\activate     (Windows)

3. Installer les dépendances :
   pip install -r requirements.txt

4. Appliquer les migrations :
   python manage.py makemigrations
   python manage.py migrate

5. Lancer le serveur :
   python manage.py runserver

Utilisation
-----------
- Accéder à l’interface via http://127.0.0.1:8000/
- Se connecter avec un compte Admin ou Employé
- Naviguer dans les modules : employés, bulletins, PDF

Structure du projet
-------------------
- payroll/ : application principale
  - models.py : modèles de données
  - views.py : vues et logique métier
  - forms.py : formulaires
  - templates/ : interfaces HTML
- static/ : fichiers CSS, JS, images
- media/ : fichiers PDF générés
- manage.py : script de gestion Django

Diagrammes UML
--------------
- Diagramme de cas d’utilisation : interactions entre Admin, Employé et le système
- Diagramme de classes : structure des entités (User, Profile, Employee, Payslip…)

Auteur
------
Projet réalisé par le groupe 23 dans le cadre d’un projet académique.

Licence
-------
Ce projet est open-source et peut être utilisé librement à des fins pédagogiques ou professionnelles.

