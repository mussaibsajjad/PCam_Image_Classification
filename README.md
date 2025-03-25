# **Medical Image Classification Using PCam Dataset**

## **Project Overview**

This repository contains a deep learning project focused on classifying histopathological images of lymph node sections as metastatic (positive) or non-metastatic (negative). Using the **PatchCamelyon (PCam)** dataset, multiple models were implemented and evaluated to achieve high classification accuracy.

---

## **Key Features**

- Dataset: PatchCamelyon (PCam) dataset.
- Models Implemented:
  - ResNet18 (Pre-trained and fine-tuned)
  - VGG16 (Pre-trained and fine-tuned)
  - Custom CNN Model (built from scratch with residual blocks and inception modules)
  - Improved ResNet18 (enhanced using dropout, data augmentation, and learning rate scheduling).
- Best Model: Improved ResNet18 achieved 80% accuracy and 0.783 F1 score.

---

## **Project Structure**

- `data/`: Dataset files and subsets.
- `models/`: Saved trained models (.pth files).
- `results/`: Results and predictions.
- `scripts/`: Python scripts for training and evaluation.
- `notebooks/`: Jupyter notebooks (if applicable).
- `README.md`: Project description and usage instructions.

---

## **How to Run the Project**

### **1. Clone the Repository**

```bash
git clone https://github.com/your-username/PCam_Image_Classification.git
cd PCam_Image_Classification
```

### **2. Install Dependencies**

```bash
pip install -r requirements.txt
```

### **3. Prepare the Dataset**

- Download the dataset from [PCam GitHub](https://github.com/basveeling/pcam).
- Place the `.h5` files in the `data/` directory.
- Create subsets for training and testing:
  ```bash
  python scripts/create_subset.py
  ```

### **4. Train the Models**

- Train ResNet18:
  ```bash
  python scripts/train_resnet18.py
  ```
- Train VGG16:
  ```bash
  python scripts/train_vgg16.py
  ```
- Train Custom Model:
  ```bash
  python scripts/train_custom_model.py
  ```
- Improve ResNet18:
  ```bash
  python scripts/improve_resnet18.py
  ```

### **5. Validate Models**

- Evaluate all models on validation data:
  ```bash
  python scripts/validate_models.py
  ```

### **6. Test Predictions**

- Generate predictions on the test dataset:
  ```bash
  python scripts/test_predictions.py
  ```
- Predictions will be saved to `results/test_predictions.txt`.

---

