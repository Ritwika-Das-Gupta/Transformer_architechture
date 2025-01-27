# Transformer Architecture - Custom Implementation

This repository contains a small transformer model built from scratch. The transformer model is based on the original architecture described in the paper [Attention is All You Need](https://arxiv.org/abs/1706.03762). It is designed to handle sequence-to-sequence tasks with self-attention mechanisms and position-wise feedforward networks.

## Overview

The Transformer model is composed of two main parts:
1. **Encoder**: Processes the input sequence to generate a context-aware representation.
2. **Decoder**: Uses the encoder's output to generate the final output sequence.

### Key Components:
- **Self-Attention**: Allows the model to focus on different parts of the input sequence when making predictions.
- **Multi-Head Attention**: Provides multiple attention mechanisms to learn different relationships between words in a sentence.
- **Position Encoding**: Adds information about the position of tokens in a sequence.
- **Feedforward Networks**: Processes each token independently through a simple neural network.
- **Layer Normalization**: Helps in stabilizing training and speeds up convergence.

## Model Architecture

The transformer consists of:
- **N Encoder Layers**
- **N Decoder Layers**

### Encoder Layer
Each encoder layer has two main sub-layers:
1. Multi-Head Self-Attention
2. Position-wise Feedforward Network

### Decoder Layer
Each decoder layer has three main sub-layers:
1. Multi-Head Self-Attention
2. Multi-Head Attention (with encoder output)
3. Position-wise Feedforward Network

Each sub-layer in both the encoder and decoder uses residual connections followed by layer normalization.
## Code Explanation
You will find in depth code explanation here - https://medium.com/@ritwika.work03/mastering-transformers-a-guide-to-building-the-heart-of-modern-ai-aac83bed5289
