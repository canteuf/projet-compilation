# Projet Compilation : DSL Robotique

## Description
Ce projet est un compilateur développé avec **Xtext** dans l'environnement Eclipse. Il implémente un langage spécifique pour  la conception d’une DSL destinée à définir des contrôleurs robotiques . Ce dépôt contient les fichiers source du langage, les configurations Eclipse, et les scripts de build nécessaires.

## Prérequis
Pour exécuter ce projet, vous devez avoir installé :
- **Eclipse IDE** avec le plugin Xtext (version 2.39.0.M3).
- **Java JDK** (version 17 ou supérieure recommandée).
- **Maven** (pour la gestion des dépendances).
- Un environnement Git configuré.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Installation
1. Clonez le dépôt :
   ```bash
   git clone https://github.com/canteuf/projet-compilation.git
   ```
2. Ouvrez Eclipse et importez le projet :
   - Allez dans **File > Import > Existing Projects into Workspace**.
   - Sélectionnez le dossier `projet-compilation` comme répertoire racine.
3. Lancez la génération des artefacts Xtext :
   - Sélectionnez le fichier `GenerateRobotDsl.mwe2` dans le dossier `src/org.xtext.robotdsl` sur le menu **`Package Explorer`**.
   - Faites un clic droit sur le fichier et sélectionnez **Run As &gt; 1 MWE2 Workflow**.
4. Configurez le projet :
   - Si Maven est utilisé, exécutez :
     ```bash
     mvn clean install
     ```
   - Assurez-vous que les dépendances sont résolues.

## Utilisation
1. Pour tester le compilateur :
   - Créez un fichier avec l'extension de votre langage ( `.rbdsl`).
   - Écrivez un programme conforme à la grammaire définie dans `RobotDsl.xtext`.
   - Exécutez le compilateur via Eclipse ou en ligne de commande (voir ci-dessous).
2. Exemple de commande pour exécuter le compilateur :
   ```bash
   java -jar target/projet-compilation.jar chemin/vers/votre/fichier.rbdsl
   ```

## Structure du projet
- `src/` : Contient les fichiers source du langage Xtext (par exemple, `src/org.xtext.robotdsl`).
- `src-gen/` : Fichiers générés automatiquement par Xtext (ignorés par Git).
- `target/` : Dossier de build Maven (ignoré par Git).
- `.gitignore` : Liste des fichiers/dossiers à ignorer par Git.
- `pom.xml` : Fichier de configuration Maven (si applicable).

## Contribution
1. Forkez le dépôt.
2. Créez une branche pour votre fonctionnalité :
   ```bash
   git checkout -b feature/nouvelle-fonctionnalite
   ```
3. Validez vos modifications et poussez :
   ```bash
   git commit -m "Ajout de nouvelle fonctionnalité"
   git push origin feature/nouvelle-fonctionnalite
   ```
4. Créez une pull request sur GitHub.
   
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Cloner le projet (En tant que `Collaborateur`)

Suivez ces étapes pour cloner le projet sur votre machine :

1. **Ouvrez un terminal** (ou Git Bash sur Windows).
2. **Clonez le dépôt** en exécutant :

   ```bash
   git clone https://github.com/canteuf/projet-compilation.git
   ```
   - Si vous utilisez SSH (recommandé pour les contributeurs), utilisez :

     ```bash
     git clone git@github.com:canteuf/projet-compilation.git
     ```

     Assurez-vous d'avoir configuré votre clé SSH dans GitHub (voir ce guide).
3. **Accédez au répertoire du projet** :

   ```bash
   cd projet-compilation
   ```

## Configurer le projet dans Eclipse

1. **Ouvrez Eclipse** et importez le projet :
   - Allez dans **File &gt; Import &gt; Existing Projects into Workspace**.
   - Sélectionnez le dossier `projet-compilation` (le répertoire où vous avez cloné le dépôt) comme répertoire racine.
   - Cliquez sur **Finish** pour importer tous les sous-projets Xtext.
2. **Générez les artefacts Xtext** :
   - Sélectionnez le fichier `GenerateRobotDsl.mwe2` dans le dossier `src/org.xtext.robotdsl` sur le menu **`Package Explorer`**.
   - Faites un clic droit sur le fichier et sélectionnez **Run As &gt; 1 MWE2 Workflow**.
3. **Configurez les dépendances** (si Maven est utilisé) :
   - Dans le terminal, à la racine du projet, exécutez :

     ```bash
     mvn clean install
     ```
   - Assurez-vous que toutes les dépendances sont téléchargées.
4. **Vérifiez la configuration** :
   - Assurez-vous que le projet compile sans erreur dans Eclipse.
   - Si des erreurs apparaissent, vérifiez que le JDK et le plugin Xtext sont correctement configurés.

## Contribuer au projet

1. **Créez une branche pour vos modifications** :

   ```bash
   git checkout -b feature/votre-fonctionnalite
   ```
2. **Ajoutez et validez vos modifications** :

   ```bash
   git add .
   git commit -m "Description de vos modifications"
   ```
3. **Poussez votre branche vers GitHub** :

   ```bash
   git push origin feature/votre-fonctionnalite
   ```
4. **Créez une pull request** :
   - Allez sur `https://github.com/canteuf/projet-compilation`.
   - Cliquez sur **New Pull Request** et sélectionnez votre branche.
   - Soumettez la pull request pour révision.
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Structure du projet

- `src/` : Contient les fichiers source du langage Xtext (par exemple, `src/org.xtext.robotdsl`).
- `src-gen/` : Fichiers générés automatiquement par Xtext (ignorés par Git).
- `target/` : Dossier de build Maven (ignoré par Git).
- `.gitignore` : Liste des fichiers/dossiers à ignorer par Git.
- `pom.xml` : Fichier de configuration Maven (si applicable).

## Problèmes courants

- **Erreur de clonage** : Vérifiez que vous avez accès au dépôt. Contactez \[votre nom ou pseudo GitHub\] pour être ajouté comme collaborateur.
- **Erreur SSH** : Assurez-vous que votre clé SSH est configurée (voir ce guide).
- **Erreur Maven** : Exécutez `mvn clean install` pour résoudre les dépendances. Vérifiez que Maven est installé et configuré.

## Contact

Pour toute question, contactez [https://github.com/canteuf/projet-compilation/issues].
