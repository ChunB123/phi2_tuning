# Enhancing Small Language Models through Advanced Tuning Techniques

## Project Overview

This study focuses on the enhancement of Small Language Models (SLMs) using advanced fine-tuning techniques, specifically applied to Microsoft's Phi-2 model. Unlike traditional research that predominantly focuses on Large Language Models (LLMs), our project highlights the potential of SLMs to perform complex tasks such as in-context learning and algorithmic reasoning. This shift challenges the notion that only LLMs can excel in these areas, potentially democratizing access to advanced AI capabilities.

## Project Structure

### Data_Preprocessing
This directory contains scripts and utilities for pre-processing the training data for both instruction tuning and symbol tuning. It also includes the preparation of evaluation data across various testing scenarios:
- `With instruction and Label`: Data prepared with both instructions and labels.
- `With instruction and Symbol`: Data where labels are replaced with symbols.
- `Without instruction and Symbol`: Data with no instructions, only symbols.
- `Flipped Label Tasks Data`: Specific datasets prepared to test the model's ability to handle flipped labels.
- `Big Bench List function and Turing dataset`: Datasets from the Big Bench challenge focusing on list function and Turing test scenarios.

### Evaluation_Result
This folder contains the implementation of human evaluation for model performance:
- `Mistral_and_chatgpt_eval.ipynb`: Jupyter notebook for evaluating outputs from the Mistral and GPT-3.5 models.
- `Evaluation_phi_2_final.ipynb`: Jupyter notebook for evaluating the Phi-2 model and its fine-tuned versions.
- `Performance_Analysis_Manual_Evaluation.xlsx`: An Excel file summarizing the performance metrics of the models.
- Subdirectories `big bench`, `flipped data`, `in-context`: These contain CSV files with records of human evaluations across different datasets.

### Model_Training
- `phi2_instruct.ipynb`: Jupyter notebook for conducting instruction tuning on the Phi-2 model.
- `phi2_symbol.ipynb`: Jupyter notebook for conducting symbol tuning on the Phi-2 model.

## Models and Datasets

Our models and datasets are publicly posted and accessible via the following links:

### Models
- **Instruction Tuning FLAN-Phi-2**: [Hugging Face Model](https://huggingface.co/ChunB1/phi-2_OpenOrca_cot_only)
- **Symbol Tuning FLAN-Phi-2-Symbol**: [Hugging Face Model](https://huggingface.co/ChunB1/phi-2_OpenOrca_cot_only_symbol)

### Tuning Datasets
- **Instruction Tuning dataset**: [Hugging Face Dataset](https://huggingface.co/datasets/ChunB1/OpenOrca_cot_only)
- **Symbol Tuning dataset**: [Hugging Face Dataset](https://huggingface.co/datasets/ChunB1/phi-2-symbol-100k-en-512)

### Evaluation Datasets
- **Big Bench Testing Data**: [Hugging Face Dataset](https://huggingface.co/datasets/AlanYky/big-bench-list-function-turing-330)
- **Classification Datasets**: These include various classification tasks such as Hate Detection, Offensive Language Detection, Subjectivity, and Climate Topic Classification across different instructional and symbolic contexts:
  - TEH, TEO, SUBJ, CLIMATE Classification datasets available [here](https://huggingface.co/AlanYky).



## Getting Started
To get started with this project:
1. Clone the repository to your local machine.
2. Ensure you have Jupyter Notebook installed, or use Google Colab for an online setup.
3. Navigate to the `Model_Training` folder to begin training models or `Data_Preprocessing` to prepare your data sets.
4. Use the notebooks in `Evaluation_Result` to assess model performance.

## Contribution
This project is a collaborative effort by Alan Yang, and Michael Xu. Each member has contributed equally to the project
