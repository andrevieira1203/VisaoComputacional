# Computer Vision : Facial Emotion Detection and Classification

## Description

This repository contains the work developed for the **Computer Vision** course, with the goal of implementing a **Convolutional Neural Network (CNN)** capable of **detecting and classifying human emotions** from facial images, using the **FER-2013** (*Facial Expression Recognition*) dataset.

The project covers the full pipeline from building and training the initial model, to a documented final version, and a real-time application using a camera feed.

---

## Repository Structure

```
VisaoComputacional/
│
├── initial_model.ipynb       # First version of the CNN model
├── model_commented.ipynb     # Final model with detailed comments
├── camara.ipynb              # Real-time emotion detection via camera
└── README.md                 # Project documentation
```

---

## Notebooks

### `initial_model.ipynb`
Development and training of the first CNN version. Includes the initial data preprocessing pipeline, network architecture, and evaluation of results.

### `model_commented.ipynb`
Improved and fully documented version of the model, with explanatory comments throughout the code. Ideal for understanding the architectural decisions and results obtained.

### `camara.ipynb`
Practical application of the trained model in **real time**, using the device's camera to detect faces and classify the expressed emotions.

---

## Dataset — FER-2013

The **FER-2013** (*Facial Expression Recognition 2013*) is a widely used public dataset for facial expression recognition tasks.

| Property | Detail |
|---|---|
| Images | ~35,000 grayscale images |
| Resolution | 48×48 pixels |
| Classes | 7 emotions |
| Source | [Kaggle / FER-2013](https://www.kaggle.com/datasets/msambare/fer2013) |

**Emotion classes:**
- 😠 Angry
- 🤢 Disgust
- 😨 Fear
- 😊 Happy
- 😐 Neutral
- 😢 Sad
- 😲 Surprise

---

## Model Architecture

The model is based on a **Convolutional Neural Network (CNN)** with the following general characteristics:

- Convolutional layers for facial feature extraction
- Pooling layers for dimensionality reduction
- Dropout for regularization and overfitting prevention
- Fully connected (dense) layers for final classification
- **Softmax** activation on the output layer (7 classes)

---

## Technologies & Libraries

- **Python 3**
- **Jupyter Notebook**
- `tensorflow` / `keras` — CNN construction and training
- `opencv-python` — real-time video capture and face detection
- `numpy`, `pandas` — data manipulation
- `matplotlib`, `seaborn` — results visualization

---

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/andrevieira1203/VisaoComputacional.git
   cd VisaoComputacional
   ```

2. Install dependencies:
   ```bash
   pip install tensorflow keras opencv-python numpy pandas matplotlib seaborn jupyter
   ```

3. Download the FER-2013 dataset from [Kaggle](https://www.kaggle.com/datasets/msambare/fer2013) and place it in the root of the project.

4. Run the notebooks in the following order:
   ```bash
   # 1. Initial model training
   jupyter notebook initial_model.ipynb

   # 2. Commented and improved version
   jupyter notebook model_commented.ipynb

   # 3. Real-time camera testing
   jupyter notebook camara.ipynb
   ```

> For `camara.ipynb`, a working camera and correctly installed OpenCV drivers are required.

---

## Languages

| Language | Percentage |
|---|---|
| Jupyter Notebook | 100% |

---.
