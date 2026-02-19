# Goal: Make faster kernels with Reinforcement Learning

## 🎯 Overview
We now add some small amount of LoRA weights to GPT-OSS so we only need to train those, instead of training on the full model.

## 🛠️ Tech Stack & Optimization
* **Base Model:** GPT-OSS (20B)
* **Framework:** Unsloth
* **Technique:** GRPO Reinforcement Learning
* **Precision:** 4-bit NF4

## 💡 Key Features & Learning Objectives
* **Optimized Fine-Tuning**: Efficient implementation with LoRA rank $r=16$ and $\alpha=16*2$.
* **Memory Management**: Optimized to run on consumer-grade hardware with significant VRAM reduction.
* **Speedup**: Leveraging Unsloth kernels for up to 2x-3x faster training and inference.

## 📊 Performance Benchmarks (Estimated)
* **VRAM Usage:** Free T4 (16GB)
* **Training Speed:** 2x speedup using Unsloth kernels.
* **Evaluation:** High performance on standard benchmarks like GSM8K and MMLU.

## 🚀 How to Use
1.  **Environment:** `pip install unsloth vllm trl`
2.  **Run:** Open `gpt-oss-(20B)-GRPO.ipynb` and execute cells.
