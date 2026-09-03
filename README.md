# CIFAR-10 Image Classification with PyTorch

## 📖 Overview
A beginner-friendly implementation of image classification on the CIFAR-10 dataset using a simple CNN model built with PyTorch. This is my first deep learning project to get familiar with the PyTorch workflow.

## 🎯 Results
- **Test accuracy**: 75.2% (after 20 epochs)
- **Training time**: ~12 min on Google Colab (GPU)
- **Best epoch**: Epoch 18

## 🛠️ Model Architecture
- 3 Conv layers + 2 MaxPool + 2 Fully Connected layers
- ReLU activation, Batch Normalization, Dropout (0.2)
- Optimizer: SGD with momentum, lr=0.001, momentum=0.9
- Loss: CrossEntropyLoss

## 📚 What I Learned
1. **PyTorch training pipeline**: DataLoader → Model definition → Loss function → Optimizer → Training loop → Evaluation
2. **How to use GPU**: `device = torch.device("cuda" if torch.cuda.is_available() else "cpu")`
3. **Common issues**: 
   - Overfitting when training too many epochs → solved with Dropout
   - Learning rate too high → loss oscillates → reduced lr from 0.01 to 0.001
4. **How to visualize**: training/validation loss curves, confusion matrix

## 📁 Project Structure
