La base de données CIFAR-10 se compose de 60 000 images couleur 32x32 dans 10 classes, avec 6 000 images par classe. Il y a 50 000 images d'apprentissage et 10 000 images de test.
L'ensemble de données est divisé en données d'apprentissage et données test, les données test contient exactement 1000 images sélectionnées au hasard dans chaque classe.
Les données d’apprentissage contiennent les images restantes dans un ordre aléatoire, les données d’apprentissage contiennent exactement 5000 images de chaque classe.

J'ai utilisé le même modèle (LeNet) utilisé dans l'exemple (LeNet-MNIST), pour comparer une deuxième fois avec les résultats sur un autre Dataset (Dans notre cas CIFAR-10).

Les résultats obtenus sont pas satisfisant, et pour EPOCHS = 10, les données test donne une accuracy = 0.63 et les données train donne une accuracy = 0.74,
Et lorsque on augmente la valeur de EPOCHS, on remarque que la différence entre accuracy des données test et accuracy des données train augmente aussi, 
ce qui nous montre une mouvaise génération de notre model sur ce Dataset.

Remarque : vous pouvez utilisé grid-search pour avoir les meilleurs hyperparamètres pour le modèle, ce qui augmentera l'accuracy obtenu
