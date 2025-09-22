# sms-spam-detection-zero-shot-GPT-vs-BERT
Comparative study of spam SMS detection using zero-shot LLMs (GPT-4o) and fine-tuned Transformer models (DistilBERT, RoBERTa). Includes EDA, model training, evaluation on F1 score with precision–recall trade-offs for real-world deployment.


# Spam SMS Detection with LLMs and Transformers

This project compares **zero-shot LLMs** with **fine-tuned Transformer models** for detecting spam SMS messages.  
It explores trade-offs between **accuracy, efficiency, and labeled data availability** in real-world NLP tasks.  

## 📌 Project Overview
- Dataset: **5,574 SMS messages** labeled as spam (13.4%) or ham (legitimate).  
- Methods:
  - **EDA**: N-gram word clouds, message length distribution to identify spam patterns  
  - **Zero-Shot LLM**: GPT-4o with prompt engineering  
  - **Fine-Tuned Transformers**: DistilBERT, RoBERTa  

## ⚙️ Models & Results

| Model                     | Precision | Recall | F1 Score |
|----------------------------|-----------|--------|----------|
| GPT-4o (zero-shot)         | 0.8045    | 0.9664 | 0.8780   |
| DistilBERT (fine-tuned)    | 0.9726    | 0.9530 | 0.9627   |
| RoBERTa (fine-tuned)       | 0.9931    | 0.9597 | 0.9761   |


## 📊 Key Insights
- Spam messages often contain terms like **“cash”**, **“prize”**, and **“customer service.”**  
- Precision vs Recall trade-off:  
  - High recall → safer (fewer missed spam), but more false positives.  
  - High precision → fewer false alarms, but risk of missing spam.  
- **Deployment Recommendation**:  
  - RoBERTa for accuracy-critical applications  
  - GPT-4o zero-shot for quick prototyping with no labeled data  
