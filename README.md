GPT from Scratch — A Math-First, Minimal Transformer Implementation

This repository is a from-scratch implementation of a nano-GPT-style language model, built step by step with the explicit goal of understanding every moving part of modern transformers — not just using them.

The project starts from raw text (Tiny Shakespeare) and walks all the way through:

tokenization

embeddings

batching and context windows

self-attention

transformer blocks

training with cross-entropy loss

autoregressive text generation

The emphasis is clarity over performance, understanding over abstraction, and math before frameworks.

Project Philosophy

Most tutorials jump quickly between frameworks, abstractions, and environments, which makes it hard to build a coherent mental model.

This project intentionally takes the opposite approach:

- One idea at a time
- Why before how
- Math and shapes explicitly tracked
- Minimal code, no magic
- Everything built from first principles

Where possible, components are first implemented conceptually (or in NumPy) before being expressed in PyTorch.

What This Project Covers
1. Data & Tokenization

Character-level tokenization

Vocabulary construction

Encoding and decoding

Train/validation splits

2. Batching & Context Windows

(B, T) input/target construction

Next-token prediction logic

Sliding context windows

Why batching works the way it does

3. Embeddings (Explained, Not Assumed)

Token embeddings

Positional embeddings

Why embeddings are high-dimensional

How embeddings learn meaning geometrically

4. Self-Attention (From the Ground Up)

Query, Key, Value projections

Attention weights (B, T, T)

Causal masking

Softmax intuition

Shape-by-shape verification

5. Transformer Block

LayerNorm

Residual connections

Feed-forward networks

Why these pieces exist (not just how)

6. Training Loop

Cross-entropy loss

Backpropagation

Gradient flow

Loss curves and stability

Why training works at all

7. Autoregressive Generation

Sampling tokens step by step

Conditioning on context

Turning logits into probabilities

Producing coherent text

What This Is Not

- Not a production-ready GPT
- Not an optimized or large-scale model
- Not a framework tutorial

This is a learning artifact, not a benchmark.

Why This Exists

Understanding transformers deeply requires:

tracking tensor shapes,

knowing where probabilities come from,

seeing how loss flows backward,

and recognizing how meaning emerges from linear algebra.

This repo is meant to serve as:

a personal reference

a teaching artifact

a conceptual bridge between math and modern NLP

Who This Is For

- Learners who want to truly understand GPT
- People frustrated by “black-box” tutorials
- Anyone curious how attention actually works
- Engineers who value first-principles thinking

