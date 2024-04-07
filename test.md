# Étape 1 : Création des 4 environnements au niveau de Anaconda Navigator:
- Ouvrir anaconda navigator et créez les 4 environnements suivants :
1. yolov7-cpu-env
2. yolov7-gpu-env
3. yolov8-cpu-env
4. yolov8-gpu-env

# Étape 2 : 
Ouvrir anaconda prompt
- activate yolov7-cpu-env
- git clone https://github.com/pHidayatullah/yolov7.git
- ren yolov7 yolov7-cpu
- cd yolov7-cpu
- pip install -r requirements.txt
- COPIER LE FICHIER YOLOV7.pt à partir de (https://github.com/pHidayatullah/yolov7?tab=readme-ov-file) dans le même dossier du projet (C:\yolov7-cpu) et excéutez la commande suivante :
- python detect.py --weights yolov7.pt --source inference\images\bus.jpg
- python detect.py --weights yolov7.pt --source 0
- C:\Users\hrehouma\AppData\Local\anaconda3\envs\yolov7-cpu-env\Lib\site-packages\cv2





# Suppression (optionnel)
- Pour supprimer : rmdir /s /q yolov7
- rmdir /s /q chemin_du_répertoire ou rd /s /q chemin_du_répertoire



