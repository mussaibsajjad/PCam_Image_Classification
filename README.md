# PCam_Image_Classification
Medical Image Classification Using PCam Dataset

Project Overview

This project implements deep learning models to classify histopathology images from the PCam dataset as metastatic (positive) or non-metastatic (negative). Multiple models were developed, including ResNet18, VGG16, and a custom CNN, with an improved ResNet18 achieving the best results.

Key Features

Dataset: PatchCamelyon (PCam) dataset.

Models Implemented:

ResNet18 (Pre-trained and fine-tuned)

VGG16 (Pre-trained and fine-tuned)

Custom CNN Model (built from scratch with residual blocks and inception modules)

Improved ResNet18 (enhanced using dropout, data augmentation, and learning rate scheduling).

Best Model: Improved ResNet18 achieved 80% accuracy and 0.783 F1 score.

Results

Model

Accuracy

Precision

Recall

F1 Score

ResNet18

0.565

0.661

0.383

0.485

VGG16

0.535

0.535

1.000

0.697

Custom Model

0.520

0.520

1.000

0.684

Improved ResNet18

0.800

0.900

0.692

0.783

Project Structure

PCam_Project/
├── data/               # Dataset files and subsets
├── models/             # Saved trained models (.pth files)
├── results/            # Results and predictions
├── scripts/            # Python scripts for training and evaluation
├── notebooks/          # Jupyter notebooks (if applicable)
└── README.md           # Project description and usage instructions

How to Run the Project

1. Clone the Repository

git clone https://github.com/your-username/PCam_Image_Classification.git
cd PCam_Image_Classification

2. Install Dependencies

pip install -r requirements.txt

3. Prepare the Dataset

Download the dataset from PCam GitHub.

Place the .h5 files in the data/ directory.

Create subsets for training and testing:

python scripts/create_subset.py

4. Train the Models

Train ResNet18:

python scripts/train_resnet18.py

Train VGG16:

python scripts/train_vgg16.py

Train Custom Model:

python scripts/train_custom_model.py

Improve ResNet18:

python scripts/improve_resnet18.py

5. Validate Models

Evaluate all models on validation data:

python scripts/validate_models.py

6. Test Predictions

Generate predictions on the test dataset:

python scripts/test_predictions.py

Predictions will be saved to results/test_predictions.txt.

Trained Models

Download the trained models:

ResNet18: Download Link

VGG16: Download Link

Custom Model: Download Link

Improved ResNet18: Download Link

Acknowledgements

Dataset: PatchCamelyon (PCam)

Frameworks: PyTorch, Torchvision



