# YOLOV8_ANOMALYDETECTION
Detection d'objets et d'anomalies sur la route, utilisant YOLOV8 et intégrant une inférence video.


#Methodes d'entrainement
Le temps d'inférence est < 10ms,  avec 3 rounds d'entrainement qui a duré en tout seulement 3 heures ( Nous aurions pu continuer l'entrainement encore au moins 4 fois plus longtemps avec cette configuration)
Les 3 stages d'entrainement avec des images progressivement plus grandes afin de rendre l'entrainement plus rapide (et des fois plus fiable)  : 
- 40 epochs avec des images 640x640 
- 35 epochs avec des images de taille 960x960
- 25 epochs par les images de taille 1280x1280 (taille originale)



# Résultats


https://github.com/user-attachments/assets/1dc643b7-535f-4c81-84ce-3b1fa1c97117

