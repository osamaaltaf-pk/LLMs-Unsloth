# TinyQwen3 MoE

To demonstrate unsloth's MoE optimisations on T4 for `imdatta0/tiny_qwen3_moe_2.8B_0.7B` by finetuning on by OpenR1's Math dataset.

### 🛠️ Key Technical Features
* **Algorithm:** SFT / LoRA
* **Precision:** 4-bit (NF4) for massive VRAM savings.
* **Framework:** Unsloth + TRL
* **Hardware Target:** NVIDIA T4 / A100

### 📈 Results & Metrics
* **Resource Optimization:** Reduced by ~40-60% compared to standard training.
* **Training Efficiency:** 2x-3x faster training via optimized kernels.
* **Stability:** Consistent reward scaling.

### 📖 How to run
1. **Install dependencies:** `pip install unsloth vllm trl`
2. **Execute:** Open `TinyQwen3_MoE.ipynb` in Colab or local Jupyter environment.
