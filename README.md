# NLP-Project- Multi-Task Hinglish NLU using MuRIL

This project implements a multi-task Hinglish Natural Language Understanding (NLU) pipeline using Google's MuRIL transformer model. The system independently fine-tunes MuRIL for three social-media NLP tasks:

Sentiment Analysis
Hate Speech Detection
Sarcasm Detection


**Features**
Fine-tuning using google/muril-base-cased
Hinglish-compatible tokenization
Separate models for each NLP task
Automatic evaluation with:
Accuracy
Weighted F1-score
Classification reports
Confusion matrices
Gradio-based interactive interface
GPU/CPU compatible
Google Colab compatible


**Included Tasks**

| Task                  | Classes                       |
| --------------------- | ----------------------------- |
| Sentiment Analysis    | Negative / Neutral / Positive |
| Hate Speech Detection | Clean / Abusive               |
| Sarcasm Detection     | Literal / Sarcastic           |


**Requirements**
For Installing Depencdencies
run-
pip install -r requirements.txt


**Dataset**
