GPT from Scratch — A Math-First, Minimal Transformer Implementation

This repository contains a from-scratch implementation of a nano-GPT–style language model, built step by step with a single goal: to understand every moving part of a modern transformer, rather than simply using one.

The project began as a close follow-along of Andrej Karpathy’s “Let’s build GPT” (Tiny Shakespeare) video. Along the way, I deliberately diverged from the tutorial whenever details were abstracted away, explained informally, or hidden behind PyTorch convenience layers. Instead, I chose to rebuild each component explicitly—sticking to pure NumPy—so that every tensor operation, gradient flow, and architectural choice remains transparent and inspectable.

This is not a performance-optimized model or a framework reimplementation. It is a learning artifact designed to make the mathematics, geometry, and mechanics of transformers concrete.
