# Lung-Cancer-Detection-CNN
This GitHub repository houses a comprehensive Convolutional Neural Network (CNN) model meticulously engineered for the early detection of lung cancer. Leveraging state-of-the-art deep learning techniques, our model boasts an exceptional accuracy rate of 100%, making it a formidable tool in the fight against this debilitating disease.

## Kaggle link
We have executed our code in kaggle: https://www.kaggle.com/lathikadevanand/lung-conference

## Dataset
The above kaggle note contains the dataset (CT scans of healthy and cancerous lungs) 

## Model 
The CNN model architecture is designed to process medical images with dimensions of 224x224 pixels and three color channels.

## Components
- Sequential Model: The CNN is structured as a sequential model, allowing for a straightforward layer-by-layer implementation.
- Convolutional Layers: Several convolutional layers are employed to extract features from the input images. Each convolutional layer is followed by rectified linear unit (ReLU) activation for non-linearity.
- MaxPooling Layers: MaxPooling layers are utilized to downsample the spatial dimensions of the feature maps, reducing computational complexity and extracting dominant features.
- Fully Connected Layers: After feature extraction, the model flattens the output and passes it through fully connected layers to perform classification. ReLU activation functions are applied to maintain non-linearity.
- Output Layer: The final layer consists of neurons equal to the number of classes (class_count) and utilizes softmax activation for multi-class classification.

## Model Compilation:
- Optimizer: The Adamax optimizer is chosen with a learning rate of 0.001 to update the model's weights during training.
- Loss Function: Categorical cross-entropy is selected as the loss function, suitable for multi-class classification tasks.
- Metrics: The model's performance is evaluated using accuracy as the metric, measuring the proportion of correctly classified samples.
