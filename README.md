# Face_recognition
Dans ce projet, nous allons mettre en place un algorithme d’identification des visages dans une photographique. Pour cela, nous aborderons deux grands axes : la détection du visage d’abord, puis la vérification ou l’identification faciale. Puis que, “ la reconnaissance faciale est souvent décrite comme un processus qui implique d'abord quatre étapes; ils sont: visage détection, alignement de visages, extraction de caractéristiques et enfin reconnaissance de visage”. Jason Brownlee
1.2	Voici les étapes :
1.	La détection du visage qui consiste à (localiser, délimiter, carré, cercle);
2.	L’alignement du visage qui consiste à (normaliser, la géométrie);
3.	L’extraction de caractéristiques (extraire les traits pour la reconnaissance du visage);
4.	Reconnaissance du visage à travers le modèle;



1.3	Détection du visage 

•	Pour que cela fonctionne, nous utiliserons un modèle de fichier en cascade haarcascade en XML avec 2 paramètres (scalFactor, minNeighbors);

•	Le modèle que nous allons utiliser est performant pour la détection des visages : MTCNN(Multi-task Cascaded Convolutional Networks
•	), il est multitâche, pré entraîné avec de la vitesse et une bonne précision;
•	
•	Utiliser keras et Python
•	
•	Créer le dataset avec une taille des images : 224 x 224 px ;
•	
•	Utiliser des boucles et des fonctions avec des paramètres;
•	
•	Pour la reconnaissance faciale, nous utiliserons un modèle performant pour la vérification : VGGFace2.

La méthode consiste d'abord à détecter les visages sur des photos, puis à vérifier les visages afin de les reconnaître ou de les identifier. Donc ici, nous sommes face à deux problématiques, la détection et l'identification des visages sur des photos ou des vidéos.

Nous utiliserons les techniques de vision par ordinateur avec l’apprentissage profond afin d'obtenir un modèle performant capable de résoudre cette problématique. 

1.3.1	 Première étape :  la détection des visages

Il s'agit d’une technique d'apprentissage profond qui permet de résoudre un problème qui consiste à localiser la position de chaque visage sur des vidéos ou sur une photographie. 

Il faut les identifier tout simplement. Pour ce faire, il faut tenir compte des traits du visage, des angles,  de la lumière et tant d'autres paramètres pour la détection. Nous jouons ainsi avec la caméra, la lumière   voire la distance en utilisant des filtres pour résoudre le problème. 

1.3.2	 Comment détecter les visages sur les photos ?

Une des techniques d'apprentissage en profondeur utilisées pour cette problématique de vision ordinateur est le Réseau de neurones convolutifs en cascade multitâche ou MTCNN. 

Ce RN est utile dans la classification des images et associe plusieurs couches d’apprentissage profond dans le cadre de la détection des visages sur des photos.

Nous allons utiliser Python puis la bibliothèque MTCNN qui est notre classificateur multitâche et la bibliothèque OpenCV.

Voici le code : 


2	Reconnaissance faciale avec VGGface2  

Dans cette partie, nous abordons l’apprentissage profond avec des réseaux de neurones convolutifs VGGFace et VGGFace2 qui ont été développés par les chercheurs du Visual Geometry Group d'Oxford.

2.1	Voici les étapes :
•	Utilisation d’un modèle pré entraîné avec Keras;
•	Identification et prédiction des noms sur la vidéo et les photos;
•	Vérification le visage ;

Les techniques d'identification des visages sont multiples. Aujourd'hui la plupart des systèmes de reconnaissance faciale possèdent une base de données gigantesque où une étude de comparaison est effectuée. 

C’est le cas de la Chine. Allez savoir la “RGPD” ce qu’on en fait. Voici le procédé, les outils et les appareils scannent les visages ensuite les comparent dans une base de données. 

Grâce à cela, nous pouvons faire aussi un mappage un à plusieurs pour un visage donné à travers une base de données connue.

Le modèle VGGface réalise l’identification faciale grâce à un ensemble de données annotées de comparaison par vision par ordinateur. Il “a été décrit par Omkar Parkhi dans l'article de 2015 intitulé Deep Face Reconnaissance”. 

Notre architecture de réseaux de neurones profonds utilise cet ensemble de données annotées avec plusieurs couches et des fonctions d'activation relu, Softmax et pooling. 

Le modèle VGGFace2 est expérimenté dans cet article dans un grand ensemble de données contenant 3,31 millions d'images de 9131 sujets, avec une moyenne de 362,6 images pour chaque sujet.

