# 🌟 Transfer Learning Image Classification Pipeline

📋 **Project Overview**  
This project implements a transfer learning pipeline in Google Colab for image classification using pre-trained deep learning models. It supports multiple datasets (Flowers, CIFAR-10, Cats vs Dogs, manual upload, and a quick demo with dummy data) with an interactive selection interface, making it ideal for beginners and advanced users exploring computer vision.

🎯 **Objectives**  
- Utilize pre-trained models for efficient image classification  
- Support multiple datasets with varying sizes and complexities  
- Provide an interactive dataset selection for ease of use  
- Achieve high accuracy with minimal setup (e.g., ~85% on CIFAR-10, ~90% on Flowers)  
- Offer visualizations for training progress and results  
- Ensure modular, beginner-friendly code with clear documentation  

📊 **Dataset Information**  
**Datasets**: Flowers, CIFAR-10, Cats vs Dogs, Manual Upload, Dummy Data  

- **Flowers**:  
  - Size: 230MB, 5 classes (daisy, dandelion, roses, sunflowers, tulips)  
  - Dimensions: Variable (resized to 224x224)  
- **CIFAR-10**:  
  - Size: 170MB, 10 classes (e.g., plane, car, bird)  
  - Dimensions: 32x32x3 (RGB)  
- **Cats vs Dogs**:  
  - Size: 500MB, 2 classes (cats, dogs)  
  - Dimensions: Variable (resized to 224x224)  
- **Manual Upload**: Custom user-provided images  
- **Dummy Data**: Synthetic data for quick testing  
**Target Output**: Multi-class/binary classification  
**Techniques**: Transfer learning with pre-trained models, data augmentation, fine-tuning  

🔧 **Technical Implementation**  
📌 **Pipeline Architecture**  
- Pre-trained model (e.g., ResNet, VGG) with fine-tuned layers  
- Data augmentation: Random flips, rotations, and normalization  
- Interactive dataset selection with user prompts  
- Modular functions for data loading, training, and evaluation  

🧹 **Data Preprocessing**  
- **Flowers/Cats vs Dogs**: Resizing, random crops, flips, normalization  
- **CIFAR-10**: Normalization (mean=0.5, std=0.5)  
- **Manual Upload**: User-defined preprocessing  
- **Dummy Data**: Synthetic image generation  

⚙️ **Training Configuration**  
- Optimizer: Adam or SGD (configurable)  
- Loss Function: CrossEntropyLoss  
- Regularization: Dropout, weight decay  
- Hardware: CPU/GPU support in Colab  

📏 **Evaluation Metrics**  
- Overall accuracy and per-class performance  
- Training loss/accuracy curves  
- Sample prediction visualizations  

📊 **Visualizations**  
- Real-time training progress with loss/accuracy plots  
- Sample image predictions with ground truth labels  

🚀 **Getting Started**  
**Prerequisites**  
- Google Colab account  
- Python 3.8+, TensorFlow/Keras, Kaggle API (for Cats vs Dogs)  

**Installation**  
Clone the repository:  
```bash
git clone https://github.com/arsalan-computer/009-Transfer-Learning-Pipeline.git
cd 009-Transfer-Learning-Pipeline
```

**Running the Code**  
Open in Colab and run:  
```python
# Interactive mode
model, results = interactive_dataset_selection()

# Direct dataset selection
model, results = run_transfer_learning_pipeline('flowers')  # Recommended
model, results = run_transfer_learning_pipeline('cifar10')
model, history = create_quick_demo()  # No download
```

📈 **Results**  
- **Flowers**: ~90% accuracy in ~10 minutes  
- **CIFAR-10**: ~85% accuracy in ~5 minutes  
- **Cats vs Dogs**: ~95% accuracy in ~15 minutes  
- **Model Size**: Varies by pre-trained model (~25-150MB)  
- **GPU Memory**: <2GB in Colab  

🙌 **Acknowledgments**  
- TensorFlow/Keras for deep learning framework  
- Dataset providers: Flowers, CIFAR-10, Kaggle (Cats vs Dogs)  
- Google Colab for free GPU resources
