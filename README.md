# Mission : Etudier la faisabilité d'un moteur de classification d'articles
## Comment allez-vous procéder ?
Cette mission suit un scénario de projet professionnel.

Vous pouvez suivre les étapes pour vous aider à réaliser vos livrables.

Avant de démarrer, nous vous conseillons de :
- lire toute la mission et ses documents liés ;
- prendre des notes sur ce que vous avez compris ;
- consulter les étapes pour vous guider ; 
- préparer une liste de questions pour votre première session de mentorat.

## Prêt à mener la mission ?
Vous êtes Data Scientist au sein de l’entreprise "__Place de marché__”, qui souhaite lancer une marketplace e-commerce.

Sur cette place de marché anglophone, des vendeurs proposent des articles à des acheteurs en postant une photo et une description.

Pour l'instant, l'attribution de la catégorie d'un article est effectuée manuellement par les vendeurs, et est donc peu fiable. De plus, le volume des articles est pour l’instant très petit.

Pour rendre l’expérience utilisateur des vendeurs (faciliter la mise en ligne de nouveaux articles) et des acheteurs (faciliter la recherche de produits) la plus fluide possible, et dans l'optique d'un passage à l'échelle,  __il devient nécessaire d'automatiser cette tâche d‘attribution de la catégorie__.

__Linda__, Lead Data Scientist, vous demande donc d'étudier la faisabilité d'un __moteur de classification__ des articles en différentes catégories, à partir du texte (en anglais) et de l’image comme dans l’illustration ci-dessous.

![articles image](https://user.oc-static.com/upload/2023/03/30/1680170799854_Data%20Scientist-P6-01%20%281%29.png)

Une image et un texte décrivant un produit mènent à une flèche vers un label, pour illustrer l'assignation automatique.

Voici le mail qu’elle vous a envoyé.

>__De :__ Linda  
>__À :__ moi  
>__Objet :__ démarrage de la mission
>
>Bonjour, 
>
>Merci pour ton aide sur ce projet !
>
>Ta mission sera de réaliser __une étude de faisabilité d'un moteur de classification automatique__ d’articles, en utilisant leur image et leur description sur le jeu de données d'articles disponible dans la première pièce jointe de ce mail.
>
>Pourrais-tu __analyser__ les __descriptions textuelles__ et les __images des produits__, au travers des étapes suivantes : 
>- Un __prétraitement__ des données texte et image 
>- Une __extraction__ de features 
>- Une __réduction__ en 2 dimensions, afin de projeter les produits sur un graphique 2D, sous la forme de points dont la couleur correspondra à la catégorie réelle 
>- Une __analyse__ du __graphique__ afin de conclure, à l’aide des descriptions ou des images, sur la __faisabilité de regrouper automatiquement__ des produits de même catégorie 
>- Une réalisation d’une __mesure pour confirmer ton analyse visuelle__, en calculant la similarité entre les catégories réelles et les catégories issues d’une segmentation en clusters
>
>Pourrais-tu nous démontrer ainsi la faisabilité de regrouper automatiquement des produits de même catégorie ?
>
>Afin d’extraire les __features image__, il sera nécessaire de mettre en œuvre :
>- un algorithme de type SIFT / ORB / SURF ;
>- un algorithme de type CNN Transfer Learning.
>
>Afin d’extraire les __features texte__, il sera nécessaire de mettre en œuvre : 
>- deux approches de type bag-of-words, comptage simple de mots et Tf-idf ;
>- une approche de type word/sentence embedding classique avec Word2Vec (ou Glove ou FastText) ;
>- une approche de type word/sentence embedding avec BERT ;
>- une approche de type word/sentence embedding avec USE (Universal Sentence Encoder).
>
>Pour t’aider, en deuxième pièce jointe, tu trouveras un __exemple__ de Notebook mettant en œuvre les approches d’extraction de features d’images sur un autre dataset.
>
>Merci encore,  
>Linda
>
>PS : J’ai bien vérifié qu’il n’y avait aucune contrainte de propriété intellectuelle sur les données et les images.
>
>Pièces jointes : 
>- PJ 1 : [Jeu de données d’articles](https://s3-eu-west-1.amazonaws.com/static.oc-static.com/prod/courses/files/Parcours_data_scientist/Projet+-+Textimage+DAS+V2/Dataset+projet+pre%CC%81traitement+textes+images.zip)
>- PJ 2 : [Notebook d’extraction de features d’images et d’étude de faisabilité](https://s3.eu-west-1.amazonaws.com/course.oc-static.com/projects/Data_Scientist_P6/Weather_Images_CNN_Transfer_Learning_Stage_1_feasibility_V1.0.ipynb)

Pour l’approche de type SIFT, n’hésitez pas à consulter le webinaire disponible dans les [ressources](https://openclassrooms.com/projects/1503/resources).
