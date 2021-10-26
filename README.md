# DCGAN
Deep Convolutional Generative Adversarial Network DCGAN, ce modele a apporté une contribution significative à l’équilibre entre l’entrainement GAN et son architecture 
convolutive. Bien que les réseaux convolutifs aient déjà été utilisés dans l’architecture GAN, DCGAN propose une architecture personnalisée. 
c’est la première architecture GAN capable de générer des images de haute
résolution. DCGAN c’est la «version image» de la mise en œuvre la plus fondamentale des GAN. Cette architecture exploite essentiellement les réseaux de neurones à
convolution profonde. Nous utilisons le jeu de données célébrité dans ce test. célébrité a 202 599 images
de visage au format RGB. Chaque valeur de pixel est comprise entre 0 et 255. Dans l’expérience, la valeur de pixel est mise à l’échelle à [-1, 1]. Nos expériences sont
faites avec une taille de lot de 64, Adam comme optimiseur avec un taux d’apprentissage de 0,0002. Dans l’étape d’échantillonnage de l’image. La taille du vecteur
aléatoire z a été fixée à 100. Après un apprentissage de 5 époques. Les pertes des
réseaux sont calculées avec l’entropie croisée tout au long du processus d’apprentissage, l’expérience contient deux parties, Dans la première expérience, le système 
est testé en utilisant la fonction d’activation TanH et
nous lançons une deuxième expérience en testant avec la fonction Sin, nous avons utilisé la fonction d’activation
périodique, et plus précisément la fonction d’activation sinusoïde dans la deuxième
expérience, Les fonctions d’activation sinusoïdale ont été largement ignorées et sont
considérées comme difficiles à entraîner, mais ce problème peut ne pas être grave
lorsque les données sont dominées par des composants à basse fréquence (ce qui est
attendu pour de nombreux ensembles de données du monde réel). L’apprentissage
est plus facile dans ce type. Dans cette expérience, nous
avons mélangé des activations périodiques et non périodiques. Nous n’utilisons la
fonction sin que pour la sortie du générateur et et les autres couches conservent la
structure du DCGAN d’origine.
