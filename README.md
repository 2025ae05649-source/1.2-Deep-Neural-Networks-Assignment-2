# Deep-Neural-Networks-Assignment-2


# CNN Question:


<img width="1033" height="482" alt="image" src="https://github.com/user-attachments/assets/dec535bd-66e1-4214-af52-1206968e6db6" />


<img width="1019" height="406" alt="image" src="https://github.com/user-attachments/assets/d5964d62-3112-4d42-afa8-3345f7109385" />

analysis:
The transfer learning model (ResNet50) outperforms the custom CNN across all metrics,
demonstrating that ImageNet pre-trained features transfer effectively to the Cats vs Dogs
binary classification task. ResNet50 converges faster, achieving lower loss within fewer
epochs due to its pre-learned hierarchical representations (edges, textures, shapes),
while the custom CNN must learn all features from scratch with limited data.

Global Average Pooling significantly reduces overfitting in both models by eliminating
large fully-connected layers that would contain millions of parameters. GAP enforces
spatial feature learning by averaging each feature map into a single value, acting as a
structural regularizer. This is evident from the smaller gap between training and
validation accuracy compared to Flatten+Dense architectures.

Computationally, the custom CNN has far fewer total parameters but requires longer training
to achieve competitive accuracy. ResNet50, despite its large frozen parameter count, trains
quickly since only the classification head is updated. Transfer learning is particularly
effective here because ImageNet contains animal categories, making the learned features
highly relevant for distinguishing cats from dogs. The convergence behavior shows ResNet50
reaches near-optimal performance within 2-3 epochs while the custom CNN needs 15+ epochs


# RNN Question: 
## Assignment Overview

### This assignment implements and compares two approaches for time series forecasting:

GRU using Keras/TensorFlow with 2 stacked layers
Transformer encoder using Keras layers with custom positional encoding
Framework: Keras/TensorFlow
Dataset: Apple (AAPL) Stock Prices from Yahoo Finance

<img width="1020" height="657" alt="image" src="https://github.com/user-attachments/assets/2d994662-4b8b-4b3a-a1b3-a9abe4019de2" />

<img width="968" height="675" alt="image" src="https://github.com/user-attachments/assets/d7990c25-33f8-4bdf-a44b-cd0eedf60b37" />


