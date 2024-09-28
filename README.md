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
| GPT2     | 0.124   | 0.1004     | 
| t5-small     | 0.7526     | 0.7612    |
| facebook/bart-base     | 0.6239    |0.8321    | 

### Model Files
Model and it's files are Uploaded on Kaggle for now 
- t5-small - https://www.kaggle.com/models/hritik619916/t5-small
- GPT2 - https://www.kaggle.com/models/hritik619916/gpt2
- Bart - https://www.kaggle.com/models/hritik619916/bart-new

## Update
-Added T5 model used further ,on HuggingFace as well,
-T5 - https://huggingface.co/Hritik619916/t5-small-model


## App

We have created Gradio Apps for the T5 Model

- T5 small - https://huggingface.co/spaces/Hritik619916/Capstone-Email-QA

### Model Weights for Gradio 
- T5 - https://huggingface.co/Hritik619916/t5-small-model





# Question Answer on AIML

The project focuses on developing and fine-tuning a GPT model to answer questions reagarding the AIML course only, focusing on generating accurate and relevant answers for the following questions.

## Dataset

The dataset used for the project is  [AIML QA Data](https://www.kaggle.com/datasets/hritik619916/new-qa-dataset).

The preprocessing in this task is primarily involved in formatting the training dataset to an appropriate prompt format.

## Models

The pre-trained model used for this Dataset is [GPT2](https://huggingface.co/openai-community/gpt2)


| Model | Rouge - 1 | Rogue - 2 | Rogue - L | 
|-----------------|-----------------|-----------------|-----------------|
| GPT2     | 0.34790018989021654   | 0.18205649943032873   | 0.2913203003549229   |


### Model Files
Model and it's files are Uploaded on HuggingFace
- GPT2 - https://huggingface.co/Hritik619916/QA_GPT2


## App

We have created Gradio Apps for the finetuned GPT2 Model

- GPT2 - https://huggingface.co/spaces/Hritik619916/Capstone-Email-QA

### Model Weights for Gradio 
- GPT2 - https://huggingface.co/Hritik619916/QA_GPT2


## ROUGE Scores Explanation:

- **ROUGE-1** measures the overlap of unigrams (single words) between the generated and reference summaries. Higher scores indicate better performance in capturing essential words.

- **ROUGE-2** evaluates the overlap of bigrams (two consecutive words). It provides insight into how well the model captures pairs of words.

- **ROUGE-L** assesses the longest common subsequence between the generated and reference summaries. It reflects the fluency and coherence of the generated text.

## Evaluation Metrics

Each of these metrics can be evaluated in terms of:

- **Precision**: The fraction of n-grams in the generated summary that are also in the reference summary.

- **Recall**: The fraction of n-grams in the reference summary that are also in the generated summary.

- **F1 Score**: The harmonic mean of precision and recall, providing a balanced measure.





