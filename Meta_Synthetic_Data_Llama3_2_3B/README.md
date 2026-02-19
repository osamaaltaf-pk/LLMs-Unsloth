# Meta Synthetic Data Llama3 2 (3B)

## 🎯 Overview
A high-performance implementation of Meta Synthetic Data Llama3 2 (3B) using Unsloth. This method optimizes memory and speed for 2026-scale LLM workloads.

## 🛠️ Tech Stack & Optimization
* **Base Model:** Llama 3.2
* **Framework:** Unsloth
* **Technique:** Fine-Tuning
* **Precision:** 4-bit NF4

## 💡 Key Features & Learning Objectives
* **Optimized Fine-Tuning**: Efficient implementation with LoRA rank $r=16$ and $\alpha=16$.
* **Memory Management**: Optimized to run on consumer-grade hardware with significant VRAM reduction.
* **Speedup**: Leveraging Unsloth kernels for up to 2x-3x faster training and inference.

## 📊 Performance Benchmarks (Estimated)
* **VRAM Usage:** Free T4 (16GB)
* **Training Speed:** 2x speedup using Unsloth kernels.
* **Evaluation:** High performance on standard benchmarks like GSM8K and MMLU.

## 🚀 How to Use
1.  **Environment:** `pip install unsloth vllm trl`
2.  **Run:** Open `Meta_Synthetic_Data_Llama3_2_(3B).ipynb` and execute cells.
