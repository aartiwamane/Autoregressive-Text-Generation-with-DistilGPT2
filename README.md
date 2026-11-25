# Autoregressive Text Generation with DistilGPT2

## Overview

This project demonstrates **autoregressive text generation** using the pretrained DistilGPT2 language model from Hugging Face Transformers.

The implementation accepts a text prompt and generates a continuation using a pretrained causal language model. It introduces the fundamentals of Large Language Model (LLM) inference and demonstrates how transformer-based models can be used for natural language generation.

## Objectives

- Understand the fundamentals of autoregressive language generation.
- Explore pretrained transformer-based language models.
- Implement text generation using the Hugging Face Transformers pipeline.
- Understand prompt-based inference and token generation.
- Experiment with deterministic text generation.

## Technologies Used

- **Programming Language:** Python
- **Deep Learning Framework:** PyTorch
- **NLP Library:** Hugging Face Transformers
- **Pretrained Model:** DistilGPT2

## How It Works

The implementation follows these steps:

1. **Pipeline Initialization:** Loads the pretrained DistilGPT2 model using the Hugging Face `pipeline()` API.
2. **Prompt Definition:** Provides an initial text sequence as input.
3. **Text Generation:** Generates additional tokens based on the supplied prompt.
4. **Decoding Strategy:** Uses greedy decoding (`do_sample=False`) to select the highest-probability next token at each generation step.
5. **Output Display:** Retrieves and displays the generated text.

## Implementation Details

| Parameter | Description |
|---|---|
| `text-generation` | Specifies the NLP task |
| `distilgpt2` | Pretrained language model |
| `max_new_tokens=30` | Maximum number of new tokens |
| `do_sample=False` | Enables deterministic greedy decoding |
| `pad_token_id` | Uses the EOS token as the padding token |

## Project Structure

```text
Autoregressive-Text-Generation-with-DistilGPT2/
│
├── 6_LLM_Autoregressive.py
├── requirements.txt
└── README.md
```

## Installation

Clone the repository:

```bash
git clone https://github.com/USERNAME/Autoregressive-Text-Generation-with-DistilGPT2.git
```

Navigate to the project directory:

```bash
cd Autoregressive-Text-Generation-with-DistilGPT2
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Execution

Run the Python script:

```bash
python 6_LLM_Autoregressive.py
```

The pretrained model is downloaded automatically when required. An internet connection is needed for the initial model download.

## Learning Outcomes

- Understanding autoregressive text generation.
- Familiarity with pretrained causal language models.
- Practical experience with Hugging Face Transformers.
- Understanding prompt-based LLM inference.
- Introduction to decoding strategies in language generation.

## Scope and Limitations

This project is an introductory implementation of text generation using a pretrained model. It does not involve training or fine-tuning a language model.

The generation quality and contextual capabilities are limited by the underlying DistilGPT2 model.

## Future Enhancements

- Experiment with temperature-based sampling.
- Implement Top-K and Top-P sampling.
- Accept dynamic user prompts.
- Compare different pretrained language models.
- Explore custom autoregressive decoding.

## Author

**Aarti Wamane**

M.Tech Computer Engineering | Machine Learning | Deep Learning | Natural Language Processing

GitHub: https://github.com/aartiwamane

LinkedIn: https://linkedin.com/in/aarti-wamane-5276562a6
