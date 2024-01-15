
# Text Summarizer using Google PEGASUS - Hugging Face

## Overview

This project implements a text summarizer model based on Google's PEGASUS, fine-tuned on the CNN/Daily Mail dataset and Samsumdata. The model can generate concise summaries of given articles or texts.

## Base Model Architecture

The base PEGASUS model architecture consists of a transformer-based neural network with self-attention mechanisms. For detailed information on the architecture, refer to the [PEGASUS paper](https://arxiv.org/abs/1912.08777).

The Pegasus model was proposed in PEGASUS: Pre-training with Extracted Gap-sentences for Abstractive Summarization by Jingqing Zhang, Yao Zhao, Mohammad Saleh and Peter J. Liu on Dec 18, 2019.

According to the abstract,

Pegasus’ pretraining task is intentionally similar to summarization: important sentences are removed/masked from an input document and are generated together as one output sequence from the remaining sentences, similar to an extractive summary.
Pegasus achieves SOTA summarization performance on all 12 downstream tasks, as measured by ROUGE and human eval.
