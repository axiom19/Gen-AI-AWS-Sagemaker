# Fine-Tuning a Generative AI Model for Dialogue Summarization

This Jupyter notebook demonstrates how to fine-tune an existing large language model (LLM) to improve its performance on dialogue summarization tasks. 

## Contents

The notebook covers:

- Loading and preprocessing the [DialogSum dataset](https://huggingface.co/datasets/knkarthick/dialogsum) 
- Setting up the pre-trained [FLAN-T5 model](https://huggingface.co/google/flan-t5-base)
- Performing full fine-tuning of the model
- Evaluating the fine-tuned model qualitatively and quantitatively (using ROUGE metrics)
- Implementing Parameter Efficient Fine-Tuning (PEFT) using LoRA
- Comparing performance of the original, fully fine-tuned, and PEFT models

## Key Techniques

- Full model fine-tuning
- Parameter Efficient Fine-Tuning (PEFT) with LoRA
- ROUGE evaluation metrics
- Hugging Face Transformers and Datasets libraries

## Results

The notebook demonstrates significant improvements in dialogue summarization performance using both full fine-tuning and PEFT approaches, with PEFT achieving comparable results to full fine-tuning while being more computationally efficient.

## Requirements
Python 3.x
PyTorch
Transformers
Datasets
PEFT
Evaluate
pandas
numpy


