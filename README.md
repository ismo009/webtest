# Jeu de l'oie - par JINNOV pour l'EPNAK

Un projet Flutter pour un jeu interactif.

## Fonctionnalités

- **Navigation** : Utilisation de `GoRouter` pour une navigation fluide entre les pages.
- **Pages principales** :
  - **Accueil** : Menu principal avec accès aux règles et thématiques.
  - **Règles** : Affichage des règles du jeu.
  - **Thématiques** : Liste des thématiques disponibles.
  - **Questions** : Affichage des questions par thématique.
  - **Détail des questions** : Vue détaillée d'une question avec réponses.
- **Personnalisation** :
  - Thèmes de couleur spécifiques pour chaque catégorie.
  - Utilisation d'une police personnalisée (`Roboto`).
- **Accessibilité** :
  - Lecture des questions et réponses avec `flutter_tts`.
  - Affichage des réponses avec une option pour agrandir le texte.
- **Données dynamiques** :
  - Chargement des questions et réponses depuis un fichier JSON.
- **Interface utilisateur** :
  - Boutons personnalisés.
  - Images de fond et logo.
  - Texte de version affiché en bas de l'écran.

## Prérequis

- [Flutter](https://flutter.dev/docs/get-started/install) doit être installé sur votre machine.
- Assurez-vous d'avoir les dépendances nécessaires en exécutant :
  ```bash
  flutter pub get
Gestion des questions
Les questions et réponses sont stockées dans un fichier JSON situé dans le dossier assets/data. Voici comment les gérer :

### Gestion des questions

#### Modifier une question existante
1. Ouvrez le fichier `assets/data/questions_categorized.json`.
2. Recherchez la catégorie et la question que vous souhaitez modifier.
3. Modifiez le texte de la question ou des réponses directement dans le fichier JSON.
4. Enregistrez vos modifications.

#### Ajouter une nouvelle question
1. Ouvrez le fichier `assets/data/questions_categorized.json`.
2. Trouvez la catégorie à laquelle vous souhaitez ajouter une question.
3. Ajoutez une nouvelle entrée dans la liste des questions. Exemple :
    ```json
    {
         "question": "Quel est le capital de la France ?",
         "answers": ["Paris", "Lyon", "Marseille"],
         "correctAnswer": "Paris"
    }
    ```
4. Enregistrez vos modifications.

#### Supprimer une question
1. Ouvrez le fichier `assets/data/questions_categorized.json`.
2. Recherchez la catégorie et la question que vous souhaitez supprimer.
3. Supprimez l'entrée correspondante. Exemple :
    ```json
    {
         "question": "Quel est le capital de la France ?",
         "answers": ["Paris", "Lyon", "Marseille"],
         "correctAnswer": "Paris"
    }
    ```
4. Enregistrez vos modifications.

#### Tester vos modifications
1. Lancez l'application en exécutant :
    ```bash
    flutter run
    ```
2. Vérifiez que les modifications sont correctement reflétées dans l'application.

### Génération de QR Code

Pour générer un QR code pointant vers une URL ou une ressource spécifique, suivez ces étapes :

1. Rendez-vous sur l'[outil en ligne gratuit d'Adobe QR Code Generator](https://www.adobe.com/fr/express/feature/image/qr-code-generator).
2. Entrez l'URL ou le texte que vous souhaitez encoder dans le QR code (lien de chaque question).
3. Personnalisez le design du QR code si nécessaire.
4. Téléchargez le QR code généré.
5. Intégrez-le dans votre projet ou partagez-le selon vos besoins.

## Conctact
- Julian BREUILLER : breuillerjulian6gmail.com
- Ismael DE LA ROSA PÉREZ : delarossaperezismael@gmail.com