# Fine-Tune FLAN-T5 with Reinforcement Learning (PPO) and PEFT to Generate Less-Toxic Summaries

This repository contains a Jupyter Notebook for fine-tuning a FLAN-T5 model to generate less toxic content using Meta AI's hate speech reward model. The reward model is a binary classifier that predicts either "not hate" or "hate" for the given text. The fine-tuning process leverages Proximal Policy Optimization (PPO) to reduce the model's toxicity.

## Table of Contents
- [1 - Set up Kernel and Required Dependencies](#1---set-up-kernel-and-required-dependencies)
- [2 - Load FLAN-T5 Model, Prepare Reward Model and Toxicity Evaluator](#2---load-flan-t5-model-prepare-reward-model-and-toxicity-evaluator)
  - [2.1 - Load Data and FLAN-T5 Model Fine-Tuned with Summarization Instruction](#21---load-data-and-flan-t5-model-fine-tuned-with-summarization-instruction)
  - [2.2 - Prepare Reward Model](#22---prepare-reward-model)
  - [2.3 - Evaluate Toxicity](#23---evaluate-toxicity)
- [3 - Perform Fine-Tuning to Detoxify the Summaries](#3---perform-fine-tuning-to-detoxify-the-summaries)
  - [3.1 - Initialize `PPOTrainer`](#31---initialize-ppotrainer)
  - [3.2 - Fine-Tune the Model](#32---fine-tune-the-model)
  - [3.3 - Evaluate the Model Quantitatively](#33---evaluate-the-model-quantitatively)
  - [3.4 - Evaluate the Model Qualitatively](#34---evaluate-the-model-qualitatively)

## 1 - Set up Kernel and Required Dependencies
Ensure the correct kernel is chosen to run the notebook. Check the details of the kernel and instance type as needed.

## 2 - Load FLAN-T5 Model, Prepare Reward Model and Toxicity Evaluator
### 2.1 - Load Data and FLAN-T5 Model Fine-Tuned with Summarization Instruction
Load the necessary datasets and the pre-trained FLAN-T5 model fine-tuned for summarization tasks.

### 2.2 - Prepare Reward Model
Prepare the hate speech reward model to classify the generated text as "not hate" or "hate".

### 2.3 - Evaluate Toxicity
Implement methods to evaluate the toxicity levels of the generated summaries.

## 3 - Perform Fine-Tuning to Detoxify the Summaries
### 3.1 - Initialize `PPOTrainer`
Set up the `PPOTrainer` with the appropriate configurations for the fine-tuning process.

### 3.2 - Fine-Tune the Model
Use PPO to fine-tune the FLAN-T5 model, aiming to reduce the toxicity of the generated summaries.

### 3.3 - Evaluate the Model Quantitatively
Assess the fine-tuned model's performance using quantitative metrics.

### 3.4 - Evaluate the Model Qualitatively
Perform qualitative evaluations to ensure the generated summaries are less toxic and contextually accurate.

## Getting Started
1. Clone this repository.
2. Install the required dependencies listed in `requirements.txt`.
3. Open the `Detoxify Summaries Lab.ipynb` notebook.
4. Follow the instructions in the notebook to fine-tune the model.

## Dependencies
- Python 3.x
- Jupyter Notebook
- Transformers (Hugging Face)
- Proximal Policy Optimization (PPO) implementation
- Meta AI's Hate Speech Reward Model

## Contributing
Feel free to submit issues or pull requests if you find any bugs or have suggestions for improvements.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

