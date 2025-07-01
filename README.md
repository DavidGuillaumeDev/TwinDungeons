# TwinDungeons

## Description

Ce dépôt contient la documentation technique du projet (nom du projet). Il détaille l'architecture, les composants principaux et les instructions de compilation pour générer l'exécutable Windows via Unreal Engine 5.

## Prérequis

* Unreal Engine 5.x
* Visual Studio 2022 (avec toolchain C++)
* Git

## Installation & Setup

1. Clonez le dépôt :

   ```bash
   ```

git clone [https://github.com/votre-organisation/nom-du-projet.git](https://github.com/votre-organisation/nom-du-projet.git)
cd nom-du-projet

````
2. Regénérez les fichiers projet Visual Studio :
   ```bash
UnrealEditor.exe nom-du-projet.uproject -projectfiles
````

3. Ouvrez le `.sln` dans Visual Studio et compilez.

## Packaging Windows

1. Ouvrez le projet dans l'éditeur UE5.
2. Vérifiez que tous les Blueprints sont à jour (Graph → Refresh All Nodes).
3. Depuis le menu **File → Package Project → Windows → Windows (64-bit)**.
4. Récupérez le `.exe` dans le dossier \`

   ```
   <path>/WindowsNoEditor/nom-du-projet/Binaries/Win64
   ```

## Architecture technique

* **C++** : Logique métier et structures de données (`USTRUCT`, `UCLASS`).
* **Blueprints** : Systèmes de quêtes, UI (`WB_QuestObjective`, `WB_QuestGiver`, etc.).
* **Assets** : Contenu graphique et audio dans le dossier `Content/`.

## Contribution

1. Ouvrez une issue pour discuter des modifications.
2. Créez une branche `feature/votre-fonctionnalité`.
3. Soumettez un pull request.

## Licence

Ce projet est sous licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus de détails.
