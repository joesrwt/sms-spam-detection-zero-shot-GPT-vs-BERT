# sms-spam-detection-zero-shot-GPT-vs-BERT

![Project Title](Image%2022-9-2568%20BE%20at%2017.31.jpeg) 

## 📑 Project Slides

You can view the full slide deck here:  
[👉 202509_SpamDetection_slide.pdf](202509_SpamDetection_slide.pdf) 


# Spam SMS Detection with LLMs and Transformers

This project compares **zero-shot LLMs** with **fine-tuned Transformer models** for detecting spam SMS messages.  
It explores trade-offs between **accuracy, efficiency, and labeled data availability** in real-world NLP tasks.  


## 📊 Key Insights
- Spam messages often contain terms like **“cash”**, **“prize”**, and **“customer service.”**  
- Precision vs Recall trade-off:  
  - High recall → safer (fewer missed spam), but more false positives.  
  - High precision → fewer false alarms, but risk of missing spam.  
- **Deployment Recommendation**:  
  - RoBERTa for accuracy-critical applications  
  - GPT-4o zero-shot for quick prototyping with no labeled data  
