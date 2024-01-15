# Text Summarizer using Google PEGASUS - Hugging Face

## Overview

This project implements a text summarizer model based on Google's PEGASUS, fine-tuned on the CNN/Daily Mail dataset and Samsumdata. The model can generate concise summaries of given articles or texts.

## Base Model Architecture

The PEGASUS model architecture is based on a transformer neural network with self-attention mechanisms. For detailed information, please refer to the [PEGASUS paper](https://arxiv.org/abs/1912.08777).

The Pegasus model was proposed in the paper titled "PEGASUS: Pre-training with Extracted Gap-sentences for Abstractive Summarization" by Jingqing Zhang, Yao Zhao, Mohammad Saleh, and Peter J. Liu on Dec 18, 2019.

According to the abstract:
Pegasus’ pretraining task is intentionally similar to summarization: important sentences are removed/masked from an input document and are generated together as one output sequence from the remaining sentences, similar to an extractive summary.
Pegasus achieves state-of-the-art summarization performance on all 12 downstream tasks, as measured by ROUGE and human evaluation.

### App Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/syam-m/Text-Summarization-Project.git
    cd Text-Summarization-Project

    ```

2. **Install dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

3. **Run the Docker image:** 

    Once the Docker image is launched, it will automatically start the app.py file. Open the provided UI host path in your browser window to test the summarizer with your input of choice.

    #### Navigate to the directory containing the Dockerfile

    ```bash
    cd path/to/Text-Summarization-Project
    ```

    #### Build the Docker image

    ```bash
    docker build -t text-summarizer
    ```

    #### Run the Docker container

    ```bash
    docker run -p 8000:8000 text-summarizer
    
    ```



### Future Developments:

I plan to diversify training datasets, introduce domain-specific corpora for robustness. Optimize hyperparameters more as per domain requirements, experiment with model architectures, and will explore transfer learning techniques. I also want to develop advanced MLOPS pipelines for continuous model monitoring, updates, and effortless cloud orchestration. I will also implement adversarial training for robustness against input variations.

