# YOLOV8_ANOMALYDETECTION
Detection d'objets et d'anomalies sur la route, utilisant YOLOV8 et intégrant une inférence video.


# Methodes d'entrainement
Le temps d'inférence est < 10ms,  avec 3 rounds d'entrainement qui a duré en tout seulement 3 heures ( Nous aurions pu continuer l'entrainement encore au moins 4 fois plus longtemps avec cette configuration)
Les 3 stages d'entrainement avec des images progressivement plus grandes afin de rendre l'entrainement plus rapide (et plus efficace)  : 
- 40 epochs avec des images 640x640 
- 35 epochs avec des images de taille 960x960
- 25 epochs par les images de taille 1280x1280 (taille originale)



# Résultats
Avec OpenCV on peut ensuite facilement passer des vidéos au modèle afin de detecter des objets et anomalies sur la route, voici le résulat video :

https://github.com/user-attachments/assets/1dc643b7-535f-4c81-84ce-3b1fa1c97117



# Conclusion

- Avec plus d'entrainement on pourrait facilement augmenter la performance ( on peut voir sur la video que certains objets detectés apparaissent et disparaissent) 
- On peut aussi rajouter plus de transformations sur le jeu d'entrainement, rajouter des filtres+distortions+bruit
