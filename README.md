# MNIST AUTOENCODER

### PART A: DATASET PREPARATION AND PREPROCESSING

In this part, the MNIST handwritten digit dataset is loaded using TensorFlow/Keras. The training and testing images are explored, and their dimensions are checked. Sample images are displayed to understand the dataset. Pixel values are converted into floating-point values and normalized between 0 and 1. Each 28 × 28 image is flattened into a 784-dimensional vector. The same images are used as both input and target output for training the autoencoder.

### PART B: IMPLEMENTING THE ENCODER AND DECODER

In this part, the encoder and decoder are implemented using Dense layers. The input layer accepts 784 features. The encoder compresses the input data into a smaller latent representation of 32 features. The decoder reconstructs the original 784 features from the compressed representation. ReLU activation is used in hidden layers, and Sigmoid activation is used in the output layer. Finally, the encoder, decoder, and complete autoencoder model summaries are displayed.

### PART C: COMPILING AND TRAINING THE AUTOENCODER

In this part, the autoencoder model is compiled using the Adam optimizer and binary cross-entropy loss function. The model is trained using the MNIST dataset by providing the same images as both input and target output. A batch size of 256 and 10 epochs are used for training. The model is validated using the test dataset to check its reconstruction performance. Training loss and validation loss are recorded for each epoch. Finally, the training and validation loss curves are plotted to observe the model's learning performance.

### PART D: DIMENSIONALITY REDUCTION, FEATURE LEARNING AND RECONSTRUCTION

In this part, the trained encoder is used to convert test images into lower-dimensional latent feature vectors. The original image dimension of 784 features is reduced to 32 features using the encoder. These compressed feature vectors are passed through the decoder to reconstruct the original images. The original and reconstructed images are displayed side by side for comparison. The reconstructed images are analyzed to understand how much important information is retained or lost during compression. Finally, the trained autoencoder model and reconstructed images can be saved for future use.

# 24ADI006_RAMYA-R_DL_EX_8
