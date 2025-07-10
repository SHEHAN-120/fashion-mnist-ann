# Fashion MNIST Classification using ANN

This project implements an Artificial Neural Network (ANN) in TensorFlow/Keras to classify grayscale fashion images from the Fashion MNIST dataset. The model was trained in Google Colab using TensorFlow 2.x.

---

## 🧠 Techniques Used

* **Data Normalization**: Scaled pixel values to range 0-1 for stable training.
* **Flattening**: Converted 28x28 images into 784-length vectors for ANN input.
* **Fully Connected Layers (Dense)**: Used for learning from image pixels.
* **Dropout Regularization**: Prevented overfitting by randomly dropping neurons during training.
* **ReLU Activation**: Applied in the hidden layer for non-linearity.
* **Softmax Activation**: Used in the output layer for multiclass classification.
* **Adam Optimizer**: Efficient optimizer for fast convergence.
* **Sparse Categorical Crossentropy**: Loss function suited for integer-labeled classification.

---

## 🚀 Project Responsibilities (as the Developer)

* Preprocessed and normalized the Fashion MNIST dataset.
* Designed and trained an ANN using TensorFlow 2.x.
* Tuned model parameters such as epochs, activations, and architecture.
* Evaluated the model on unseen test data.
* Saved and documented model weights.

---

## ⚡ Challenges Faced

* Choosing the right number of layers and neurons.
* Preventing overfitting while maintaining high accuracy.
* Balancing training time vs. model performance.
* Understanding the impact of dropout and activation functions.

---

## 📊 Model Performance

* **Test Accuracy**: \~88.5% after 7 epochs
* **Model Size**: Lightweight ANN with \~128 hidden units

---

## ⬆️ How to Increase Accuracy

* **Increase Epochs**: More epochs can allow the model to learn better patterns but risks overfitting.
* **Change Activation Functions**:

  * Try `tanh`, `leaky_relu` instead of `relu` for smoother gradients.
* **Add More Layers or Neurons**: Increases capacity to learn complex patterns.
* **Use CNN Instead of ANN**: CNNs perform better on images.
* **Data Augmentation**: Apply rotation, zoom, shift, etc. to create more variety.

---

## ⛔ Why Dropout is Important

* If you **remove dropout**, the model may achieve **very high training accuracy**, but test accuracy will likely **drop** due to **overfitting**.
* Dropout forces the model to generalize by randomly deactivating neurons during training.


---


