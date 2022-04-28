# Autism classification
## DNN model
The model performs three steps:
1. Fetches preprocessed ABIDE dataset using the nilearn module.
2. Extracts FC matrix from the rs-fMRI data.
3. Classifies participants using a simple DNN model (3 hidden layers) implemented in pytorch.

## CNN model
1. This model extracts correlation, covariance, and sparse inverse covariance matrices from rs-fMRI data.
2. Then it concatenates three matrices into one tensor.
3. Finally, a convolutional neural network is utilized to classify participants based on the tensor from step 2.
4. Loss values are plotted after the model is trianed.

## CapsNet model
This model extracts correlation matrices from rs-fMRI data and classifies them using a simple capsule neural network.

![Capsules](https://github.com/thisisamirv/abide/blob/main/capsnet.png "Capsules")

You can read more about CapsNets in [here](https://proceedings.neurips.cc/paper/2017/file/2cad8fa47bbef282badbb8de5374b894-Paper.pdf) 


Note: Cache and data are not uploaded, due to their huge size.
