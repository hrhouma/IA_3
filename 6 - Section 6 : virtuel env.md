# 1 - Activation de l'Environnement Virtuel pour le Projet dans WINDOWS

- Ce guide vous montre comment activer l'environnement virtuel Python pour le développement de ce projet sous Windows. 
- Les instructions sont fournies pour l'utilisation dans la ligne de commande Windows ainsi que dans Visual Studio Code.

## Prérequis

- Assurez-vous d'avoir Python et Visual Studio Code installés sur votre machine. 
- Si ce n'est pas le cas, installez-les à partir de leurs sites officiels ou à partie de Windows Store (Python) :

- Python: [python.org](https://www.python.org/downloads/)
- Visual Studio Code: [code.visualstudio.com](https://code.visualstudio.com/)

## Activation dans Windows

### 1- Installez ANACONDA :  https://www.anaconda.com/anaconda-navigator 
### 2 - Allez dans Environnements
![image](https://github.com/hrhouma/YOLO-2/assets/10111526/b42ec3ef-611a-4533-8c1f-9e6e1b782d1f)
### 3 - Créez un nouvel environnement tkinter-env (choisir votre version de python pour cet environnement python 3.9 par exemple)
![image](https://github.com/hrhouma/YOLO-2/assets/10111526/b3139f27-4e4c-4082-a993-06a9abd4c9e5)
### 4 - Lancez l'environnement (méthode 1 via le navigateur anaconda) : 
![image](https://github.com/hrhouma/YOLO-2/assets/10111526/9743bde2-69ee-4af2-908f-bb65a3e0a1f4)
![image](https://github.com/hrhouma/YOLO-2/assets/10111526/f42f6253-14cc-47b4-a9c0-22ee806b8b28) 

### 4 - Lancez l'environnement (méthode 2 via la ligne de commande) : 
4-1. Assurez vous d'avoir conda ajoutée dans vos variables d'environnements (localisez anaconda3 d'abord, dans mon cas : C:\ProgramData\anaconda3)
4-2. Excécutez les commandes suivantes : 
```powershell
cd C:\Users\Haythem\Desktop\codesPython
conda activate tkinter-env
deactivate ou conda deactivate
```
![image](https://github.com/hrhouma/YOLO-2/assets/10111526/a15dd895-0350-46d0-8f36-84307af33217)








### PowerShell

1. Ouvrez PowerShell.
2. Naviguez vers le répertoire du projet où se trouve l'environnement virtuel. Par exemple :
   ```powershell
   cd chemin\vers\votre\projet
   ```
3. Exécutez le script d'activation :
   ```powershell
   .\venv\Scripts\Activate.ps1
   ```
   Assurez-vous que votre environnement virtuel s'appelle `venv`. Sinon, remplacez `venv` par le nom correct de votre répertoire d'environnement virtuel.

### CMD

1. Ouvrez Command Prompt (CMD).
2. Naviguez vers le répertoire du projet où se trouve l'environnement virtuel. Par exemple :
   ```cmd
   cd chemin\vers\votre\projet
   ```
3. Exécutez le script d'activation :
   ```cmd
   venv\Scripts\activate.bat
   ```



# 1 - Activation de l'Environnement Virtuel pour le Projet dans Vscode

## Activation dans Visual Studio Code

1. Ouvrez Visual Studio Code.
2. Ouvrez le dossier contenant votre projet via `File > Open Folder`.
3. Ouvrez un nouveau terminal (Terminal -> New Terminal).
4. Dans le terminal, activez l'environnement virtuel en exécutant :
   ```powershell
   .\venv\Scripts\Activate.ps1
   ```
   Si vous utilisez CMD dans le terminal de VSCode, utilisez :
   ```cmd
   venv\Scripts\activate.bat
   ```

Une fois l'environnement virtuel activé, vous verrez le préfixe `(venv)` dans votre terminal, indiquant que toutes les commandes Python et pip s'exécuteront dans l'environnement virtuel.

## Problèmes Communs

- **Politiques d'exécution PowerShell**: Si vous ne pouvez pas exécuter des scripts sur votre système, vous pourriez avoir besoin de changer les politiques d'exécution avec cette commande dans PowerShell (en tant qu'administrateur) :
  ```powershell
  Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
  ```
- **Erreur d'activation**: Assurez-vous que le chemin d'accès au script d'activation est correct et que vous utilisez le bon script pour votre terminal (PowerShell vs CMD).

Pour plus d'informations, veuillez consulter la documentation officielle de Python sur la gestion des environnements virtuels.
```

Ce README est structuré pour aider les utilisateurs à naviguer facilement dans le processus d'activation de l'environnement virtuel, avec des sections claires et des commandes spécifiques pour différentes interfaces. Il inclut également des conseils pour résoudre les erreurs communes.
