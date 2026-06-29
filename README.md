# AI-Powered Python Code Bug Detection

## Overview

This project implements an AI-based system for detecting bugs in Python source code using deep learning. The goal is to classify Python code snippets as either **clean** or **buggy** by leveraging both a custom Bidirectional Long Short-Term Memory (BiLSTM) model and a pretrained transformer model (CodeBERT).

The project demonstrates the complete machine learning workflow, including synthetic dataset generation, data preprocessing, model training, evaluation, and interactive inference through a Gradio web interface.

---

## Features

* Detects whether a Python code snippet contains a bug.
* Implements two deep learning approaches:

  * 1. Bidirectional LSTM (BiLSTM)
  * 2. CodeBERT Transformer
* Generates a synthetic dataset by introducing realistic bugs into clean Python programs.
* Evaluates models using:

  * Accuracy
  * Precision
  * Recall
  * F1 Score
  * Confusion Matrix
* Includes an interactive Gradio interface for testing custom Python code.

---

## Project Workflow

1. Collect clean Python functions.
2. Generate buggy versions using automated mutation techniques.
3. Tokenize the source code.
4. Train deep learning models.
5. Evaluate model performance.
6. Predict whether new code is clean or buggy.

---

## Technologies Used

* Python
* PyTorch
* Hugging Face Transformers
* CodeBERT
* Scikit-learn
* Gradio
* Google Colab
* NumPy
* Pandas
* Matplotlib

---

## Dataset

This project uses a **synthetically generated dataset**. A collection of clean Python functions is used as the base dataset, and realistic programming bugs are automatically introduced to create buggy samples. The resulting dataset is labeled into two classes:

* Clean Code
* Buggy Code

This approach enables supervised learning without requiring a manually annotated bug dataset.

---

## Model Architecture

### BiLSTM

* Token Embedding Layer
* Bidirectional LSTM
* Fully Connected Layer
* Binary Classification Output

### CodeBERT

* Pretrained CodeBERT Encoder
* Classification Head
* Binary Prediction

---

## Evaluation Metrics

The models are evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

These metrics provide a comprehensive assessment of the bug detection performance.

---

## Future Improvements

The current implementation serves as a proof of concept. Future work includes:

* Training on real-world bug datasets such as BugsInPy and CodeSearchNet.
* Detecting specific bug categories rather than binary classification.
* Identifying the exact line containing the bug.
* Providing explanations for detected bugs.
* Suggesting automatic fixes.
* Deploying the model as a web application or IDE extension.

---

## Repository Structure

```
AI-Code-Bug-Detection/
│
├── bug_detection_colab.ipynb
├── README.md
├── requirements.txt
└── LICENSE
```

---

## How to Run

1. Clone the repository.

```bash
git clone https://github.com/your-username/AI-Code-Bug-Detection.git
```

2. Open the notebook in Google Colab or Jupyter Notebook.

3. Install the required dependencies.

```bash
pip install -r requirements.txt
```

4. Run all notebook cells to train the models and launch the Gradio interface.

---

## Results

The project compares the performance of a custom BiLSTM model and a pretrained CodeBERT model for Python bug detection. Experimental results, evaluation metrics, and confusion matrices are presented in the notebook.

---

## License

This project is released under the MIT License.

---

## Author

**Heran Weyessa**

Artificial Intelligence and Machine Learning Enthusiast

Interested in Deep Learning, Natural Language Processing, Computer Vision, and Software Engineering.
