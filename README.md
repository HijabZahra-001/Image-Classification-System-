
# Image Classification System using Transfer Learning

A deep learning system that classifies images using Transfer Learning with MobileNetV2/ResNet50.

## Quick Overview
- **Model**: MobileNetV2 (pre-trained on ImageNet)
- **Classes**: 2-10 categories (custom dataset)
- **Accuracy**: 85-95%

## Features
- Transfer Learning with fine-tuning
- Data augmentation (rotation, zoom, flip)
- Train/Validation split (80/20)
- Confusion matrix & performance metrics
- Model saving (.h5) & loading
- Single & batch predictions

## How to Use

### 1. Setup Dataset
```
dataset/
├── class1/
│   └── images
├── class2/
│   └── images
└── class3/
    └── images
```

### 2. Install
```bash
pip install tensorflow numpy matplotlib seaborn scikit-learn Pillow
```

### 3. Train
```bash
python train.py
```

### 4. Predict
```python
classifier.predict_image('image.jpg')
```

## Output Files
- `model.h5` - Trained model
- `training_history.png` - Accuracy/Loss graphs  
- `confusion_matrix.png` - Confusion matrix
- `classification_report.txt` - Detailed report

## Requirements
- Python 3.8+
- TensorFlow 2.8+
- Matplotlib, Seaborn, Scikit-learn

**Time**: ~30 minutes to train
**Dataset**: Minimum 10 images per class
```
