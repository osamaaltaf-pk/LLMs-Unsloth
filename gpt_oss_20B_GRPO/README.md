# Reward functions

Logic and math reasoning without a separate Critic model, popularized by DeepSeek-R1.

### 🛠️ Key Technical Features
* **Algorithm:** GRPO (Reinforcement Learning)
* **Precision:** 4-bit (NF4) for massive VRAM savings.
* **Framework:** Unsloth + TRL
* **Hardware Target:** NVIDIA T4 / A100

### 📈 Results & Metrics
* **Resource Optimization:** Reduced by ~40-60% compared to standard training.
* **Training Efficiency:** 2x-3x faster training via optimized kernels.
* **Stability:** Consistent reward scaling.

### 📖 How to run
1. **Install dependencies:** `pip install unsloth vllm trl`
2. **Execute:** Open `gpt-oss-(20B)-GRPO.ipynb` in Colab or local Jupyter environment.
