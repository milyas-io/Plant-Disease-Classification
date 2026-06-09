# Plant Disease Classification using CNN and EfficientNetV2B0

This project classifies plant leaf diseases using two deep learning approaches:

1. Custom CNN model
2. Transfer learning using EfficientNetV2B0

## Dataset

The project uses the PlantVillage dataset with 15 classes.

Total images used: 20,639  
Training images: 16,512  
Validation images: 4,127  

## Previous Model: Custom CNN

The custom CNN was trained from scratch using convolutional layers, batch normalization, max pooling, dropout, flattening, dense layers, and softmax classification.

Custom CNN accuracy: 58.71%

## Updated Model: EfficientNetV2B0 Transfer Learning

The updated model uses EfficientNetV2B0 with ImageNet pre-trained weights. The classifier head was trained first, followed by controlled fine-tuning of the last EfficientNet layers.

Best fine-tuned validation accuracy: 89.65%  
Final validation accuracy: 89.18%  
Final validation loss: 0.3543  

## Final Comparison

| Model | Accuracy |
|---|---:|
| Custom CNN | 58.71% |
| EfficientNetV2B0 without fine-tuning | 87.38% |
| Fine-tuned EfficientNetV2B0 | 89.65% |

## Final Selected Model

Fine-tuned EfficientNetV2B0 was selected as the final model because it achieved the highest validation accuracy and showed better generalization.
