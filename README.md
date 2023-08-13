# DS-UA-301-Final-Presentation
A repo containing all the files and code notebooks I used for my final project
Spam Detection using Language Model Transformers

Description of the Project:

This project is focused on the implementation and evaluation of spam detection models using various datasets, encompassing both email datasets and YouTube comments. The main aim is to harness the capabilities of contemporary Language Model Transformers (LLMs) such as RoBERTa and juxtapose their performance with conventional machine learning models.

Repository and Code Structure:

The repository adheres to the following structure:
refer to https://github.com/jpmorganchase/llm-email-spam-detection for more details on the LLM and Baseline model codebase 

data/: Hosts raw, processed, and intermediary data files.

processed/: Houses the preprocessed datasets, primed for model training.
src/: Contains the comprehensive source code.

baselines/: Features the implementation of conventional machine learning models.
llms/: Dedicated to the implementation of Language Model Transformers.
outputs/: Stores saved models, logs, and other output files.

results/: Accommodates performance metrics, plots, and other evaluation results.

main.py: The primary script for executing experiments.

requirements.txt: Enumerates the Python dependencies.

Example Commands to Execute the Code:

To Train Baseline Models:
python main.py --train_baselines --dataset=email

To Train LLM (e.g., RoBERTa):
python main.py --train_llm=roberta --dataset=youtube

To Evaluate a Pre-trained Model:
python main.py --evaluate --model=roberta --dataset=youtube

Results and Observations:

The outcomes are diverse, contingent on the dataset and the model under scrutiny. Here’s a concise summary:

Traditional Models on Email Dataset:

NB: Accuracy – 95.2%, F1-Score – 94.8%
(Additional models and their results in pdf version and colab link)
RoBERTa on YouTube Dataset:

Epoch 1: Training Loss – ..., Validation Loss – ..., F1-Score – 97.2%
(Additional models and their results in pdf version and colab link)

Observations:

Language Model Transformers, with RoBERTa as a representative, demonstrated a notable uplift in performance when compared to their traditional counterparts.
Although models like Naive Bayes (NB) and Logistic Regression (LR) displayed commendable outcomes, they fell short of the nearly impeccable scores accomplished by transformer models.
The computational adversities encountered during the training phase of larger LLMs notwithstanding, the results underline their prospective advantages and the potential they present.
For an in-depth exploration, encompassing charts, plots, and a more profound interpretation of the results, kindly refer to the results/ directory.

Link to Colab:
https://colab.research.google.com/drive/1vnB4xLIBmVUpgAh-nBFBHnnG3F-Z9d-J?usp=sharing 
