# Document Image Classification

A Deep Learning project focused on classifying document images into 16 categories using EfficientNet-B2 and Transfer Learning.

## Competition Information

- Platform: Kaggle
- Task: Multiclass Document Image Classification
- Number of Classes: 16
- Training Images: 32,003
- Testing Images: 7,994

## Model Architecture

- EfficientNet-B2
- ImageNet Pretrained Weights
- Transfer Learning
- AdamW Optimizer
- Cross Entropy Loss with Label Smoothing
- Mixed Precision Training (AMP)

## Data Preprocessing

- Image path resolution
- Image integrity validation
- Aspect ratio preservation
- Resize and white padding
- Image augmentation
- Stratified train-validation split

## Performance

| Metric | Result |
|---|---:|
| Previous Public Score | 0.85152 |
| Best Public Score | **0.86198** |
| Leaderboard Rank | **28** |

## Technologies

- Python
- PyTorch
- Torchvision
- Scikit-learn
- Pandas
- NumPy
- Google Colab
- Kaggle

## Project Structure

```text
document-image-classification/
├── document_image_classification.ipynb
├── README.md
└── .gitignore
```

## Author

Naomy Athaya Jovany  
Data Science Undergraduate Student  
Institut Teknologi Sepuluh Nopember (ITS)
