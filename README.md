
# Age and Gender Detection using Deep Learning

This project predicts **age** and **gender** from facial images using deep learning models such as **VGG16** and **ResNet** with **transfer learning**. It is based on the **Adience Benchmark Dataset** and demonstrates how CNNs can accurately classify gender and estimate age groups even under challenging lighting and pose conditions.

---

## 📚 Overview

- Techniques used: Convolutional Neural Networks (CNNs), Transfer Learning, Data Augmentation  
- Dataset: Adience benchmark dataset (publicly available)  
- Accuracy achieved:  
  - Gender detection: 96.59%  
  - Age estimation: 62.73%  

---

## 🧩 Project Structure

age-gender-detection/

├── project.ipynb

├── requirements.txt # Python dependencies

├── .gitignore # Files and folders to ignore in Git

├── LICENSE # License for reuse

├── Data/adience


------

## ⚙️ Installation and Usage

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/<Bharathyalagi>/<age-and-gender-detection-using-deep-learning>.git
cd <age-and-gender-detection-using-deep-learning>
```

### 2️⃣ Clone the Repository
```bash
pip install -r requirements.txt
```

### 3️⃣ Download the Dataset

This project uses the **Adience Benchmark Dataset** for age and gender classification.

Download link:  
[https://talhassner.github.io/home/projects/Adience/Adience-data.html],

(https://talhassner.github.io/home/projects/Adience/Adience-data.html)

After downloading, place the dataset in: 
```bash
data/adience/
```

### 4️⃣ Run the Notebook
Open project.ipynb in Jupyter/kaggle/collab Notebook and run all cells step-by-step.

### Optional
## Environment and How I ran experiments

All experiments and results were produced in a Kaggle notebook environment (GPU-enabled). If you want to reproduce the results locally, use Python 3.8+ and install the dependencies from `requirements.txt`. Some functionality (GPU training) will be faster on a CUDA-enabled GPU.  
If you ran this project in a different environment, please update the environment details here.

## Evaluation and Metrics

The main evaluation metrics reported in the paper and produced by the notebook are:

**Gender Detection**
- Training accuracy: 96.59%
- Validation accuracy: 86.14%
- Epochs: 50

**Gender Detection (Augmented)**
- Training accuracy: 79.32%
- Validation accuracy: 81.25%
- Epochs: 100

**Age Detection**
- Training accuracy: 62.73%
- Validation accuracy: 58.42%
- Epochs: 200

Overall, the system performed **strongly in gender detection** due to its binary nature and the use of the Sigmoid function.  
**Age prediction** achieved moderate accuracy because of overlapping facial features among age groups, but still demonstrated solid generalization with proper data augmentation.  
Future improvements can focus on **balanced age classes**, **larger datasets**, and **custom activation or ensemble models** to further improve age prediction accuracy.

### Confusion matrix and classification report
The notebook includes code to compute and display a confusion matrix, precision, recall and F1 scores for gender classification. See the `Evaluation` section of `project.ipynb` to reproduce these plots and tables.


# Thank You




