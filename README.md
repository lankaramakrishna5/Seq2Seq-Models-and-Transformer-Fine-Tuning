# Seq2Seq Language Models for Wikipedia Title Generation

This project explores the development, training, and comparative analysis of various Sequence-to-Sequence (Seq2Seq) models for the task of generating titles for Wikipedia articles from their body text. The experiments range from implementing a custom GRU-based RNN from scratch to fine-tuning and prompting state-of-the-art Transformer models like T5 and Flan-T5.

## Table of Contents
- [Project Overview](#project-overview)
- [Key Features](#key-features)

## Project Overview

The core objective is to treat title generation as an extreme text summarization task. Given the text body of a Wikipedia article, the models are trained to generate a concise and relevant title. This repository contains the code for three main experimental stages:

1.  **Data Preprocessing:** Cleaning and preparing the Wikipedia article dataset.
2.  **RNN-based Models:** Building a baseline Seq2Seq model with a GRU-based encoder-decoder architecture from scratch using PyTorch.
3.  **Transformer-based Models:** Leveraging the Hugging Face ecosystem to fine-tune a pre-trained T5 model and perform zero-shot prompting with Flan-T5.

## Key Features

- **Custom RNN Implementation:** Seq2Seq model with a bidirectional GRU encoder and autoregressive decoder built from scratch.
- **T5 Fine-Tuning:** Fine-tuned `google/t5-small` on the dataset, demonstrating a significant performance uplift.
- **Zero-Shot Prompting:** Evaluated the effectiveness of `google/flan-t5-base` and `google/flan-t5-large` for title generation without any fine-tuning.
- **Prompt Engineering:** Systematically tested different instructional prompts to measure their impact on model performance.
- **Comparative Analysis:** Detailed performance comparison between RNN and Transformer architectures using ROUGE metrics.
- **Decoding Strategy Evaluation:** Contrasted Greedy Search and Beam Search decoding methods for latency and accuracy trade-offs.

For results and other things about the project please go through the problem statement and report pdfs..
