# Optimizer Comparison on KMNIST 🔠

A comparative analysis of deep learning optimizers - **Adam**, **RMSprop**, and **AdamW** - using a feedforward neural network on the **KMNIST** dataset. This project evaluates how different optimizers affect model accuracy, loss, and training time on handwritten Japanese Hiragana character recognition.

> 📘 Developed as part of a course in July 2025.

---

## 📌 Features

- 📈 **Benchmarking of 3 Optimizers**: Adam, RMSprop, and AdamW
- 🔁 **5-Fold Cross-Validation** for robust evaluation
- 🧪 **Randomized Hyperparameter Tuning** (learning rate, batch size)
- 🧮 Evaluation across accuracy, loss, and training efficiency
- 📊 Comparative bar plots and metric-based analysis

---

## 🧠 Dataset

Sourced from:  
**[Kuzushiji-MNIST (KMNIST)](https://github.com/rois-codh/kmnist)**  
- 10 classes of cursive Japanese Hiragana characters  
- 60,000 training images (28×28 grayscale)  
- 10,000 test images  
- Designed as a drop-in replacement for MNIST

---

## 🧠 Model Architecture

Feedforward neural network implemented in PyTorch:
- Input layer (784 features)
- 2 hidden layers with ReLU activation
- Output layer with 10 classes (Softmax)
- Loss function: `CrossEntropyLoss`
- Evaluation metrics: Accuracy, Loss, Training Time

---

## 🧪 Results Summary

| Optimizer | Best CV Accuracy | Mean Loss | Training Time |
|-----------|------------------|-----------|----------------|
| RMSprop   | **88.68%**       | 1.5763    | 51.87 seconds  |
| Adam      | 88.64%           | 1.5763    | 70.83 seconds  |
| AdamW     | 88.07%           | 1.5829    | **42.30 seconds** |

---

## 📁 Folder Structure

## 📁 Folder Structure

```bash
brain-tumor-cnn/
├── notebook/
│   ├── brain_tumor_classifier_cnn.ipynb            # Main notebook
│   └── Midterm_5502_brain_tumor_image.pdf           # PDF version of notebook
│
├── reports/
│   ├── 5502_Report_Brain_Tumor_Classification.pdf        # Final report
│   ├── 5502_Presentation_Brain_Tumor_Classification.pdf  # Final slides (PDF)
│   └── 5502_Presentation_Brain_Tumor_Classification.pptx # Raw PowerPoint
│
├── README.md

```

---

## 🔗 Related Technologies

- PyTorch  
- NumPy / Matplotlib  
- KMNIST dataset by ROIS-CODH  
- Scikit-learn (for cross-validation)

