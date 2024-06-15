# LLM Summarizer

This project demonstrates the use of a pre-trained large language model (LLM) for dialogue summarization without prompt engineering, using the FLAN-T5 model from Hugging Face. The goal is to explore various inference techniques, including zero-shot, one-shot, and few-shot, to generate summaries of dialogues from Hugging Face datasets.

## Features

- **Importing Libraries:** Setup and import required libraries including datasets and transformers.
- **Model Loading:** Load the FLAN-T5 model and tokenizer using Hugging Face's `transformers` library.
- **Base Summaries:** Generate base summaries without prompt engineering to establish a baseline.
- **Instruction Prompt Inference:** Implement zero-shot inference with an instruction prompt to enhance summary quality.
- **One-Shot and Few-Shot Inference:** Build functions for one-shot and few-shot inference to further improve summarization.
- **Generative Configuration Parameters:** Experiment with different generative configuration parameters like `do_sample`, `top_k`, `top_p`, and `temperature` to tweak the model's output.

## Usage

1. **Setup Environment:** Install the required packages using pip.
    ```bash
    pip install torch==1.13.1 torchdata==0.5.1 transformers==4.27.2 datasets==2.11.0
    ```

2. **Load Model and Tokenizer:** Use the provided code snippets to load the FLAN-T5 model and tokenizer.
    ```python
    from transformers import AutoModelForSeq2SeqLM, AutoTokenizer

    model = AutoModelForSeq2SeqLM.from_pretrained("flan-t5")
    tokenizer = AutoTokenizer.from_pretrained("flan-t5")
    ```

3. **Generate Summaries:** Use the provided functions to generate dialogue summaries with different inference techniques and configuration parameters.

## Results

- **Zero-Shot Inference:** Initial summaries without additional examples or context.
- **One-Shot Inference:** Improved summaries using a single example as context.
- **Few-Shot Inference:** Enhanced summaries using multiple examples for context.
- **Configuration Tweaks:** Different outputs by adjusting generative parameters.

## Conclusion

This project highlights the flexibility and capabilities of pre-trained LLMs like FLAN-T5 in generating concise and relevant summaries of dialogues. By experimenting with various inference techniques and configuration parameters, we can significantly improve the quality of generated summaries.

