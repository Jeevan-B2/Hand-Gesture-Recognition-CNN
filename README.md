### Hand Gesture Recognition using CNN

### 📌 Objective
Develop a hand gesture recognition model that can accurately identify and classify different hand gestures from image data to enable intuitive human-computer interaction.

### 📊 Dataset
The dataset used is the [LeapGestRecog dataset](https://www.kaggle.com/datasets/gti-upm/leapgestrecog) from Kaggle, which contains images of 10 different hand gestures performed by multiple subjects.

### 🛠️ Tools & Technologies
*   **Python**
*   **Google Colab**
*   **TensorFlow / Keras** (Deep Learning)
*   **OpenCV (cv2)** (Image Processing)
*   **Matplotlib** (Data Visualization)

### 🧠 Approach
1.  **Data Preprocessing:** Images were downloaded via KaggleHub, resized to 64x64 pixels, and normalized (scaled from 0-255 to 0-1) to improve neural network convergence.
2.  **Model Architecture:** Built a Convolutional Neural Network (CNN) using TensorFlow/Keras. The architecture includes:
    *   Two `Conv2D` layers (32 and 64 filters) with ReLU activation for feature extraction.
    *   Two `MaxPooling2D` layers to reduce spatial dimensions.
    *   A `Flatten` layer to convert 2D feature maps to 1D.
    *   A `Dense` hidden layer (128 units) with ReLU.
    *   A final `Dense` output layer with Softmax activation for multi-class classification.
3.  **Training:** The model was trained for 5 epochs using the Adam optimizer and Sparse Categorical Crossentropy loss function.

### 📈 Results
*   The model achieved an outstanding test accuracy of **99.95%**.
*   **Key Learning:** CNNs are vastly superior to traditional ML models (like SVMs) for image classification because they can automatically learn spatial hierarchies of features (edges, shapes, patterns) without needing manual flattening.
