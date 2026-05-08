# NLP-Project- Multi-Task Hinglish NLU using MuRIL

This project implements a multi-task Hinglish Natural Language Understanding (NLU) pipeline using Google's MuRIL transformer model. The system independently fine-tunes MuRIL for three social-media NLP tasks:

Sentiment Analysis
Hate Speech Detection
Sarcasm Detection


## Features

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


## Included Tasks

| Task                  | Classes                       |
| --------------------- | ----------------------------- |
| Sentiment Analysis    | Negative / Neutral / Positive |
| Hate Speech Detection | Clean / Abusive               |
| Sarcasm Detection     | Literal / Sarcastic           |


## Requirements

For Installing Depencdencies
run-
pip install -r requirements.txt


## Datasets

Datasets are in the folder "Data" folder  where all the relavant datasets are stored.
And here are the links for all the datasets that we have used:
1. Sentiment dataset- https://github.com/rsgoss/NLP_finalproj/blob/main/data/hindi-english/train_14k_split.csv
2. Hate speech dataset- https://www.kaggle.com/datasets/sharduldhekane/code-mixed-hinglish-hate-speech-detection-dataset
3. Sarcasm dataset- https://www.kaggle.com/datasets/amaan00290/hinglish-sarcasm-and-emotion-detection-dataset2025?select=sarcasm_hinghlish_dataset.csv


## Running the Project

1. Upload the notebook to Google Colab
2. Upload datasets into the data/ folder
3. Run all notebook cells sequentially


## Our Statement

We are writing to sincerely apologize for the confusion regarding our dataset during the final presentation.

As we got deeper into the implementation, we realized the new dataset we switched to was quite a mess. When we sat down to finalize our report, we found that nearly half of the sentences in hate speech about 49% were actually duplicates or incorrectly labeled and for sarcasm about 22% were Devanagari sentences. 

To make sure our results were actually reliable, we had to make some last-minute changes:

We removed all the "noise" and duplicates from the hate speech and sarcasm dataset.

The Hate Speech samples dropped by about half because of this cleanup.

The "Emotion" category was removed since it wasn't available in this specific set.

We feel really bad that we didn't explain these changes clearly during the presentation. We were so focused on trying to fix the data issues and getting the models to run that we didn't realize how much the scope had shifted until we looked at the final numbers.
