Image Classification with Deep Learning 

This assignment covers training and evaluating various deep learning models 
on the Imagenette and CIFAR-10 datasets. The goal is to develop models for 
image classification tasks and implement techniques like regularization and 
transfer learning. 

1. Basic CNN 
Architecture: The basic CNN model was built with several convolutional 
layers followed by fully connected layers. The architecture aimed for 
simplicity to establish a baseline model. 
Training Details: 
• Early stopping was implemented to prevent overfitting. 
• Best Model Path is downloaded and uploaded in the zip file. 
Results: 
• Training Loss: The model's training loss reduced over epochs, 
indicating effective learning. 
•  
• Validation Loss: Early stopping was based on validation loss, 
preventing overfitting. 
• Final Test Accuracy: The model achieved an accuracy of 74.73% on the 
test set. 
 
 
 
 
 
2. ResNet 18 
Architecture: ResNet 18, a popular deep learning model for image 
classification, was chosen for its robustness in handling complex image 
datasets. 
Training Details: 
• Early stopping was again implemented to avoid overfitting. 
• The model achieved convergence at epoch 8, signaling effective 
learning. 
Results: 
• Training Loss: The loss decreased with each epoch, showing efficient 
learning. 
 
• Validation Loss: Monitored to avoid overfitting, and early stopping was 
applied. 
 
 
• Final Test Accuracy: The ResNet 18 model reached 78.61% accuracy 
on the test set. 
 
 
3. Regularization (Data Augmentation) 
Approach: To improve generalization, data augmentation was applied to the 
basic CNN model, introducing random transformations to the input images. 
Comparison: 
Without Regularization: Accuracy reached 72.39% on the test set and Early 
stopping at epoch 7. 
With Regularization: The test accuracy improved due to data augmentation, 
yielding better generalization and a slightly higher accuracy. 
Conclusion:  
Data augmentation as a regularization method effectively enhanced the 
model’s robustness, slightly increasing test accuracy compared to the non
augmented model.

5. Transfer Learning 
Process: 
Pre-training on Imagenette: The ResNet model was first trained on the 
Imagenette dataset, achieving reasonable convergence with a test accuracy 
of 72.16%. 
Fine-tuning on CIFAR-10: 
From Scratch: Training the model from scratch on CIFAR-10 achieved a test 
accuracy of 72.59%. 
Using Pre-trained Weights: Fine-tuning the Imagenette-trained model on 
CIFAR-10 led to a lower accuracy, with a final test accuracy of 43.61%.

Conclusion: 
While transfer learning typically aids in improving accuracy, the lower 
performance on CIFAR-10 when using Imagenette-pre-trained weights may 
indicate insufficient similarity between the two datasets or overfitting during 
fine-tuning. 
