# AI-generated-text-detector
Collegiate Thesis entitled "AI-generated text vs Human-written text detection using Generative Adversarial Network (GAN)"

[cite_start]This repository contains the full manuscript, code, and supplementary materials for the thesis titled "AI-generated text vs Human-written text detection using a Generative Adversarial Network (GAN)".   

Abstract
[cite_start]In an era of rapidly developing Large Language Models (LLMs), the challenge of distinguishing between AI-generated and human-written text has become increasingly difficult. [cite_start]This study addresses this issue by using a Generative Adversarial Network (GAN) to detect AI-generated text, comparing its performance against a fine-tuned RoBERTa-based model. [cite_start]The research evaluates the effectiveness of a GAN-based discriminator, which is configured to dynamically generate diverse synthetic text samples, enabling it to better capture the subtleties of GPT-3.5 Turbo-generated text and improve classification performance.   

Key Features and Methodology
[cite_start]The project follows a three-phase evaluation framework to assess and compare the GAN-based discriminator's performance against a RoBERTa model.   

Data Acquisition and Preparation: The study uses a dataset sourced from Gaggar et al. (2023)[cite_start], consisting of approximately 400,000 AI-generated and 380,000 human-written text samples. [cite_start]The dataset is pre-processed through text cleaning and domain classification, followed by splitting into 80% training, 10% validation, and 10% testing sets.   

[cite_start]

Model Training: The core of the project involves training a GAN model, focusing on optimizing the discriminator to differentiate between human-written and AI-generated text. [cite_start]The model incorporates convolutional layers in the Discriminator and LSTM layers in the Generator for nuanced feature extraction.   

[cite_start]

Performance Evaluation: The trained GAN discriminator's ability to classify texts is measured using metrics such as accuracy and Area Under the Receiver Operating Characteristic (AUC-ROC). [cite_start]The results are then directly compared with the fine-tuned RoBERTa model.   

Results and Findings
[cite_start]The study found that the RoBERTa-base model achieved higher AUC-ROC scores across all phases, with 97.62% during training, 95.24% in validation, and 97.31% on the test set. [cite_start]In contrast, the GAN-Discriminator recorded scores of 93.03% for training, 92.71% in validation, and 92.55% on the test set. [cite_start]The non-overlapping confidence intervals of the two models indicate a statistically significant difference, supporting the conclusion that the RoBERTa-base model outperformed the GAN-Discriminator model in terms of AUC-ROC.   

[cite_start]The GAN model did, however, show effective performance in well-structured domains like Sports (AUC-ROC: 98.31%) and Business/Economics (AUC-ROC: 92.46%), while showing lower metrics in more nuanced domains such as Health (AUC-ROC: 86.79%) and Politics (AUC-ROC: 83.66%).   

Conclusions and Recommendations
[cite_start]The GAN-based approach shows promise for text classification, but the study highlights the need for further refinement to produce higher-quality synthetic text. Recommendations for future work include:   

[cite_start]Further fine-tuning of GAN hyperparameters to improve sentence generation and discriminator performance.   

[cite_start]Exploring advanced GAN architectures, such as RelGANs or WGANs, to enhance the quality and diversity of synthetic text.   

[cite_start]Augmenting the dataset with more diverse samples from multiple labeled domains to improve model generalizability.   

Authors
[cite_start]Mico Angelo Mallari    

[cite_start]Aaliyah Makayla Santos    

[cite_start]Rafael Gerard Tolentino    

[cite_start]Justin Andrie Vargas    

Adviser: Asst. [cite_start]Prof. Rochelle Lynn Lopez, DT    

[cite_start]

Date: November 2024