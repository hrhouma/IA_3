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


4-3. Autres commandes : 

-Cous commençons par la commande suivante : 
   ```bash
   conda init
   ```
- Par exemple, pour supprimer un environnement Conda, vous devez utiliser la commande `conda remove --name nom_env --all`. 
- Voici comment vous pouvez procéder étape par étape, en incluant votre demande initiale :

1. **Créer un environnement Conda** (dans votre cas, vous avez mentionné la création d'un environnement appelé `test-env`) :
   ```bash
   conda create -n test-env
   ```

2. **Lister tous les environnements Conda** pour vérifier que votre environnement a bien été créé :
   ```bash
   conda env list
   ```

3. **Activer un environnement Conda** spécifique (dans votre cas `tkinter-env`), pour travailler avec :
   ```bash
   conda activate tkinter-env
   ```

4. **Désactiver l'environnement Conda actuellement actif** :
   ```bash
   conda deactivate
   ```

5. **Supprimer un environnement Conda**. Si vous souhaitez supprimer l'environnement `test-env` que vous avez créé précédemment, utilisez :
   ```bash
   conda remove --name test-env --all
   ```

Assurez-vous d'être dans le bon dossier ou de spécifier le chemin complet si nécessaire. Si vous travaillez souvent avec des scripts ou des commandes dans des dossiers spécifiques, vous pouvez vous déplacer dans le dossier approprié en utilisant `cd` (Change Directory) dans votre terminal ou invite de commande. Dans votre cas pour aller sur le bureau dans le dossier codesPython :
```bash
cd C:\Users\Haythem\Desktop\codesPython
```

Après vous être déplacé dans le dossier, vous pouvez exécuter les commandes Conda comme décrit ci-dessus.

```powershell
conda create -n haythem-env
```
![image](https://github.com/hrhouma/YOLO-2/assets/10111526/ecc998fc-e9a2-4426-a44e-3cbff22a58e5)
```powershell
conda env list
```
![image](https://github.com/hrhouma/YOLO-2/assets/10111526/ca4d83c8-bbdc-4808-abbd-3e00b4eb280b)
```powershell
conda activate tkinter-env
```
![image](https://github.com/hrhouma/YOLO-2/assets/10111526/f26cef9f-8e00-4819-8445-94ae3bc149b8)
```powershell
 conda deactivate
```
 ![image](https://github.com/hrhouma/YOLO-2/assets/10111526/f33eeb76-2799-4e68-a4c1-643a7310972b)
 ```powershell
conda remove --name haythem-env --all
```
![image](https://github.com/hrhouma/YOLO-2/assets/10111526/253eede6-fcaf-41c8-98a3-29b28d6da8d7)






# 2 - Activation de l'Environnement Virtuel pour le Projet dans WINDOWS

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


Ce README est structuré pour aider les utilisateurs à naviguer facilement dans le processus d'activation de l'environnement virtuel, avec des sections claires et des commandes spécifiques pour différentes interfaces. Il inclut également des conseils pour résoudre les erreurs communes.


# Références utiles :
https://stackoverflow.com/questions/53995171/anaconda-conda-error-argument-command-invalid-choice-when-trying-to-update-pa
