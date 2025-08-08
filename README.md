# AI-generated-text-detector
Collegiate Thesis entitled "AI-generated text vs Human-written text detection using Generative Adversarial Network (GAN)"

---

## ✨ Abstract

> In an era of rapidly developing Large Language Models (LLMs), the challenge of distinguishing between AI-generated and human-written text has become increasingly difficult. This study addresses this issue by using a Generative Adversarial Network (GAN) to detect AI-generated text, comparing its performance against a fine-tuned RoBERTa-based model. The research evaluates the effectiveness of a GAN-based discriminator, which is configured to dynamically generate diverse synthetic text samples, enabling it to better capture the subtleties of GPT-3.5 Turbo-generated text and improve classification performance.

---

## 🛠️ Key Features and Methodology

The project follows a three-phase evaluation framework to assess and compare the GAN-based discriminator's performance against a RoBERTa model.

### 📝 Phase 1: Data Acquisition and Preparation
* **Dataset**: Sourced from Gaggar et al. (2023), consisting of ~400,000 AI-generated and ~380,000 human-written text samples.
* **Preprocessing**: The dataset is cleaned and categorized by domain.
* **Split**: The data is split into 80% training, 10% validation, and 10% testing sets.

### ⚙️ Phase 2: Model Training
* A **GAN model** is trained with the specific goal of optimizing the discriminator's ability to classify text.
* **Discriminator**: Utilizes `convolutional layers` for feature extraction.
* **Generator**: Employs `LSTM layers` to produce synthetic text.

### 📈 Phase 3: Performance Evaluation
* **Metrics**: Model performance is measured using **Accuracy** and **Area Under the Receiver Operating Characteristic (AUC-ROC)**.
* The results are directly compared to a fine-tuned **RoBERTa** model.

---

## 📊 Results and Findings

### Comparison of Model Performance
| Model | Training AUC-ROC | Validation AUC-ROC | Test Set AUC-ROC |
| :--- | :---: | :---: | :---: |
| **RoBERTa-base** | `97.62%` | `95.24%` | `97.31%` |
| **GAN-Discriminator** | `93.03%` | `92.71%` | `92.55%` |

> **Conclusion**: The RoBERTa-base model significantly outperformed the GAN-Discriminator model, with non-overlapping confidence intervals.

### GAN-Discriminator Performance by Domain
* **High Performance**:
    * Sports: `98.31% AUC-ROC`
    * Business/Economics: `92.46% AUC-ROC`
* **Lower Performance**:
    * Health: `86.79% AUC-ROC`
    * Politics: `83.66% AUC-ROC`

---

## 🚀 Conclusions and Recommendations

The GAN-based approach shows promise but requires further refinement. Recommendations for future work include:

* Fine-tuning GAN hyperparameters to improve sentence generation and discriminator performance.
* Exploring advanced GAN architectures, such as **RelGANs** or **WGANs**, to enhance the quality and diversity of synthetic text.
* Augmenting the dataset with more diverse samples to improve model generalizability.

---

## 🧑‍🎓 Authors

* Mico Angelo Mallari
* Aaliyah Makayla Santos
* Rafael Gerard Tolentino
* Justin Andrie Vargas

**Adviser:** Asst. Prof. Rochelle Lynn Lopez, DT

**Date:** November 2024