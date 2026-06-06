# DEEP-LEARNING-PROJECT_2

**COMPANY**: CODTECH IT SOLUTIONS

**NAME**: kORSIPATI MIDHILESH REDDY

**INTERN ID**: CTIS9177

**DOMAIN**: DATA SCIENCE

**BATCH DURATION**: MAY 9th, 2026 TO JUNE 6th, 2026

**MENTOR**: NEELA SANTOSH

**DEEP LEARNING PROJECT**

This project focuses on image classification using Deep Learning and TensorFlow. The primary objective is to build, train, and evaluate a Convolutional Neural Network (CNN) capable of accurately classifying images from the CIFAR-10 dataset, one of the most widely used benchmark datasets in computer vision. The project demonstrates the complete deep learning workflow, including data loading, preprocessing, model development, training, evaluation, and performance analysis.

The project begins by importing essential libraries such as TensorFlow, NumPy, and Matplotlib. These libraries provide the tools required for numerical computation, visualization, and deep learning model creation. The CIFAR-10 dataset is then loaded directly from TensorFlow’s dataset repository. This dataset contains 60,000 color images of size 32×32 pixels, divided into 10 categories: Airplane, Automobile, Bird, Cat, Deer, Dog, Frog, Horse, Ship, and Truck. Out of the total images, 50,000 are used for training and 10,000 for testing.

After loading the dataset, the project explores the structure of the data by examining the dimensions of the training and testing images and labels. Understanding the dataset is a crucial step because it helps verify that the data has been loaded correctly and is suitable for model training. To gain further insight into the dataset, a custom visualization function is created. This function displays sample images along with their corresponding class labels, allowing visual inspection of the data and helping identify the characteristics of each category.

Data preprocessing is then performed to improve the effectiveness of the learning process. Since image pixel values range from 0 to 255, they are normalized by dividing them by 255. This scales all values to the range of 0 to 1, which helps the neural network converge faster during training. The class labels are also reshaped and flattened to ensure compatibility with TensorFlow’s training functions.

The core of the project is the design and implementation of a Convolutional Neural Network (CNN) using TensorFlow’s Functional API. CNNs are particularly effective for image-related tasks because they automatically learn important visual features such as edges, textures, and shapes. The model architecture consists of multiple convolutional layers with ReLU activation functions, followed by batch normalization layers that stabilize and accelerate training. Pooling layers are included to reduce spatial dimensions while preserving important features. After feature extraction, a Global Max Pooling layer and dense neural network layers are used for classification. A dropout layer is also incorporated to reduce overfitting by randomly disabling neurons during training.

The output layer uses a Softmax activation function, producing probability scores for each of the ten classes. The model is compiled using the Adam optimizer, which is known for its efficiency and adaptive learning capabilities. The loss function selected is Sparse Categorical Crossentropy, which is suitable for multi-class classification problems where labels are represented as integers.

The model is trained in two stages. In the first stage, the network learns directly from the original dataset over multiple epochs. In the second stage, data augmentation techniques are introduced to improve model generalization. These techniques include horizontal flipping and image shifting, which create modified versions of training images. Data augmentation helps the model become more robust by exposing it to a wider variety of image patterns.

After training, the model’s performance is evaluated using several metrics and visualization techniques. Training and validation accuracy graphs are plotted to monitor learning progress and identify potential overfitting or underfitting issues. A classification report is generated to provide detailed metrics such as precision, recall, and F1-score for each class. Finally, a confusion matrix heatmap is created to visualize classification performance across all categories and identify which classes are most frequently confused.

Overall, this project demonstrates a complete deep learning image classification pipeline using TensorFlow and CNNs. It highlights important concepts such as data preprocessing, convolutional neural networks, data augmentation, model optimization, and performance evaluation, making it an excellent practical implementation of deep learning for computer vision applications.
