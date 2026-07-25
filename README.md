# 🩺 Polyp Segmentation using UNet++ with EfficientNet-B4

Automatic colorectal polyp segmentation from colonoscopy images using **UNet++** with an **EfficientNet-B4 encoder**. This project leverages deep learning for semantic segmentation to accurately identify and localize polyps in endoscopic images, aiding computer-assisted diagnosis.

---

## 📌 Overview

Colorectal cancer is one of the leading causes of cancer-related deaths worldwide. Early detection and accurate segmentation of polyps during colonoscopy can significantly improve diagnosis and treatment outcomes.

This project implements a semantic segmentation pipeline using **UNet++** with an **EfficientNet-B4** backbone. The model is trained on the **Kvasir-SEG** dataset with extensive data augmentation and evaluated using **Intersection over Union (IoU)** and **Dice Coefficient**.

---

## 🚀 Key Features

- ✅ UNet++ architecture for semantic segmentation
- ✅ EfficientNet-B4 pretrained encoder
- ✅ Dice Loss optimization
- ✅ Albumentations-based data augmentation
- ✅ AdamW optimizer with Cosine Annealing Learning Rate Scheduler
- ✅ Automatic train/validation/test split
- ✅ Performance evaluation using IoU and Dice Score
- ✅ Visualization of segmentation predictions

---

## 🛠️ Tech Stack

- Python
- PyTorch
- segmentation-models-pytorch
- Albumentations
- NumPy
- Matplotlib
- scikit-learn
- Pillow

---

## 📂 Dataset

**Dataset:** Kvasir-SEG

The Kvasir-SEG dataset contains **1,000 colonoscopy images** with corresponding manually annotated segmentation masks for colorectal polyps.

Dataset Link:

https://datasets.simula.no/kvasir-seg/

---

## 🧠 Model Architecture

- **Architecture:** UNet++
- **Encoder:** EfficientNet-B4
- **Loss Function:** Dice Loss
- **Optimizer:** AdamW
- **Learning Rate Scheduler:** Cosine Annealing LR
- **Framework:** PyTorch

---

# 📊 Training Performance

The training and validation metrics demonstrate stable convergence throughout training.

![Training History](images/training_history.png)

The model shows:

- Consistent decrease in training and validation loss
- Stable convergence during training
- High validation IoU and Dice Score
- Good generalization with only mild overfitting

---

# 🔍 Sample Predictions

### ⭐ Excellent Prediction

![Prediction Best](images/prediction_best.png)

---

### ⭐ High Accuracy Prediction

![Prediction Good](images/prediction_good.png)

---

### ⭐ Typical Prediction

![Prediction Normal](images/prediction_normal.png)

---

### ⭐ Challenging Case

![Prediction Challenging](images/prediction_challenging.png)

This example demonstrates a more difficult segmentation scenario where the model partially captures the target region. Including such examples highlights both the strengths and limitations of the model.

---

# 📈 Evaluation Metrics

The model is evaluated using:

- **Dice Coefficient**
- **Intersection over Union (IoU)**

Representative prediction results include:

| Example | IoU | Dice |
|----------|----:|-----:|
| Best Prediction | 0.984 | 0.992 |
| High Accuracy | 0.963 | 0.981 |
| Typical Case | 0.903 | 0.949 |
| Challenging Case | 0.553 | 0.712 |

> These values correspond to representative test samples and illustrate the model's performance across varying levels of difficulty.

---

# 📁 Project Structure

```text
Polyp-Segmentation/
│
├── notebook/
│   └── Polyp_Segmentation_UNetPlusPlus.ipynb
│
├── images/
│   ├── training_history.png
│   ├── prediction_best.png
│   ├── prediction_good.png
│   ├── prediction_normal.png
│   └── prediction_challenging.png
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

# ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/anikitachi/Polyp-Segmentation.git
cd Polyp-Segmentation
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Open the notebook:

```text
notebook/Polyp_Segmentation_UNetPlusPlus.ipynb
```

Run all cells to train or evaluate the model.

---

# 🔮 Future Improvements

- Attention U-Net
- DeepLabV3+
- Transformer-based segmentation models
- Hyperparameter optimization
- Mixed precision training
- Model deployment using Streamlit or Flask

---

# 👨‍💻 Author

**Anand Narayan**

B.Tech Computer Science and Engineering  
Amrita Vishwa Vidyapeetham

GitHub: https://github.com/anikitachi

---

## ⭐ If you found this project useful, consider giving the repository a star.
