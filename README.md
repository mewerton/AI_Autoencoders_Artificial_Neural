# AI_Autoencoders_Artificial_Neural
Artificial Neural - Autoencoders

O código implementa um autoencoder para reconstrução e classificação de imagens do conjunto de dados Fashion MNIST. O autoencoder é uma rede neural que aprende a codificar os dados de entrada em uma representação de menor dimensionalidade e, em seguida, decodifica essa representação de volta para reconstruir os dados originais. Isso pode ser útil para compressão de dados e remoção de ruído.

O código realiza as seguintes etapas:

Carrega o conjunto de dados Fashion MNIST e normaliza os valores dos pixels para o intervalo [0, 1].
Transforma as imagens em vetores unidimensionais (784 pixels).
Aplica ruído aos dados para criar versões ruidosas das imagens.
Cria e treina um autoencoder com 4 camadas densas para reconstruir as imagens originais.
Codifica e decodifica as imagens de teste sem ruído, visualizando algumas originais e reconstruídas.
Codifica e decodifica as imagens de teste com ruído, visualizando algumas originais e reconstruídas.
Cria e treina um classificador MLP de 3 camadas com Dropout após cada camada densa para classificar as imagens.
Avalia a acurácia do classificador nas imagens sem ruído, com ruído e nas imagens recuperadas do ruído.
As alterações feitas para melhorar a acurácia incluem a adição de camadas de Dropout após as camadas densas do classificador, o que ajuda a reduzir o overfitting durante o treinamento, e a alteração do otimizador para Adam com uma taxa de aprendizagem menor, o que pode ajudar a melhorar a convergência e a precisão do modelo.

=============================================================

The code implements an autoencoder for the reconstruction and classification of images from the Fashion MNIST dataset. An autoencoder is a neural network that learns to encode input data into a lower-dimensional representation and then decodes this representation back to reconstruct the original data. This can be useful for data compression and noise removal.

The code performs the following steps:

Loads the Fashion MNIST dataset and normalizes the pixel values to the range [0, 1].
Reshapes the images into one-dimensional vectors (784 pixels).
Applies noise to the data to create noisy versions of the images.
Creates and trains an autoencoder with 4 dense layers to reconstruct the original images.
Encodes and decodes the test images without noise, visualizing some original and reconstructed images.
Encodes and decodes the test images with noise, visualizing some original and reconstructed images.
Creates and trains a 3-layer MLP classifier with Dropout after each dense layer to classify the images.
Evaluates the classifier's accuracy on the images without noise, with noise, and on the images recovered from the noise.
The changes made to improve accuracy include adding Dropout layers after the dense layers of the classifier, which helps reduce overfitting during training, and changing the optimizer to Adam with a lower learning rate, which can help improve convergence and model accuracy.
