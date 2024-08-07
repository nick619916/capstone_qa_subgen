# AIML - QA and Email Subject Generator

QA and Email Subject Generator is a project to assess and compare how well different pre-trained  
AI models perform in NLP by focusing on two specific tasks :
-> Answer technical questions regarding AI / ML
-> Generate a Subject line for a given Email Body


# Email Subject Generator

The project focuses on developing an AI model to generate email subjects from email body content. 
It aims to create relevant and engaging subject lines automatically

## Dataset

The dataset used for the project is  [Annotated Enron Subject Line Corpus (AESLC)](https://github.com/ryanzhumich/AESLC).

- It consists of a subset of cleaned, filtered and deduplicated emails from the Enron Email Corpuswhich consists of employee email inboxes from the Enron Corporation.
* For evaluation, the data is split into development and test sets, each containing three subject lines annotated by human reviewers. This multiple-reference approach allows comprehensive assessment of the generated subjects, acknowledging the challenge of defining a single, perfect subject for each email.


## Models

The pre-trained model used for this Dataset are [t5-small](https://huggingface.co/google-t5/t5-small),[GPT2](https://huggingface.co/openai-community/gpt2),[facebook/bart-base](https://huggingface.co/facebook/bart-base)


| Model | Rouge - L | Sacrebleu | 
|-----------------|-----------------|-----------------|
| GPT2     | 0.1112   | 0.9392     | 
| t5-small     | 0.7526     | 0.7612    |
| facebook/bart-base     | 0.6239    |0.8321    | 

### Model Files
Model and it's files are Uploaded on Kaggle for now 
- t5-small - https://www.kaggle.com/models/hritik619916/t5-small
- GPT2 - https://www.kaggle.com/models/hritik619916/gpt2
- Bart - https://www.kaggle.com/models/hritik619916/bart-new


## App

We have created Gradio Apps for the T5 Model

- T5 small - https://huggingface.co/spaces/Hritik619916/email-subject-t5

### Model Weights for Gradio 
- T5 - https://huggingface.co/Hritik619916/t5-small-model



