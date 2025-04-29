# Fine-Tuning Pythia-1B for Sentiment Analysis using LoRA

This project fine-tunes the `EleutherAI/pythia-1b-deduped` model using **Parameter Efficient Fine-Tuning (PEFT)** techniques (specifically LoRA) on a subset of the **Amazon Polarity** sentiment dataset.

All steps including data loading, model setup, fine-tuning, evaluation, and hyperparameter tuning are organized into a **single notebook** for easier reproduction and review.

---

## 📄 Project File

- `Assignment_GoTG_Transformers.ipynb`:  
  Complete notebook containing:
  - Data Loading and Preprocessing
  - Model Loading and LoRA Injection
  - Base Model Fine-Tuning
  - Model Evaluation and Metrics Calculation
  - Hyperparameter Tuning Experiments (Run 1 to Run 4)

---

## 🛠 Setup Instructions

1. (Optional but recommended) Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate   # Linux/Mac
   venv\Scripts\activate      # Windows
   ```

2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

---

## 🚀 How to Run

1. Open `Assignment_GoTG_Transformers.ipynb` in Jupyter Notebook or Google Colab.
2. Run all cells sequentially to reproduce:
   - Data preparation
   - Model fine-tuning
   - Model evaluation
   - Hyperparameter tuning experiments

---

## 📊 Key Experiments Conducted

- **LoRA Fine-Tuning Hyperparameters Tuned:**
  - Learning Rate
  - LoRA Rank (r)
  - Dropout Rate
  - Number of Epochs

- **Evaluation Metrics:**
  - Sample Accuracy
  - Macro-Averaged F1 Score
  - Confusion Matrix Visualization

---

## 📈 Dataset Summary

- **Dataset**: Amazon Polarity
- **Sample Size**: 10,000 training reviews + 50 evaluation samples
- **Task**: Binary sentiment classification (Positive vs Negative)

---

## ⚡ Highlights

- Efficient LoRA-based fine-tuning reducing trainable parameters.
- Hyperparameter tuning across four structured experiments.
- Evaluation on unseen samples using F1 Score and Confusion Matrix.
- 4-bit model quantization enabled for memory optimization.

---

## 📌 Notes

- Project created as part of **Guardians of the Galaxy** team assignment.
- Base model used: `EleutherAI/pythia-1b-deduped`.
- Final best model selected after 2 epochs training with LoRA adapters.

---
