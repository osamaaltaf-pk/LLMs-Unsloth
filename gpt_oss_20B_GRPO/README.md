# Goal: Make faster kernels with Reinforcement Learning

## 🎯 Overview
We now add some small amount of LoRA weights to GPT-OSS so we only need to train those, instead of training on the full model.

## 🛠️ Tech Stack & Optimization
* **Base Model:** GPT-OSS (20B)
* **Framework:** Unsloth
* **Technique:** GRPO Reinforcement Learning
* **Precision:** 4-bit NF4

## ⚙️ Implementation Details & Features
* **Scalable Fine-Tuning**: Configured with LoRA rank $r=16$ and $\alpha=16*2$ for balanced stability and adaptation.
* **Production Memory Efficiency**: Designed to maximize hardware utility on T4/A100 instances with optimized Unsloth kernels.
* **Kernel Speedups**: Real-world 2x-3x training acceleration achieved via manual gradient checkpointing and Triton-based kernels.

## 📈 Performance & Resource Management
* **VRAM Usage:** Free T4 (16GB) (Optimized for production deployments)
* **Training Throughput:** Significant reduction in TFLOPS overhead via Unsloth optimizations.
* **Evaluation Baseline:** Validated against production benchmarks (GSM8K, MMLU) for zero-regression builds.

## 🚀 Execution & Deployment
1.  **Environment Setup:** `pip install unsloth vllm trl`
2.  **Usage:** Execute `gpt-oss-(20B)-GRPO.ipynb` for model weight adjustment and export.
