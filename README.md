# LLMs-Unsloth Implementation Hub

A centralized repository for production-ready LLM optimizations including quantization, fine-tuning (SFT/DPO/GRPO), and multimodal architecture implementations.

## 📒 Project Work & Implementations

* [Synthetic Data Hackathon](Synthetic_Data_Hackathon/README.md)
* [Whisper](Whisper/README.md)
* [Goal: Make faster kernels with Reinforcement Learning](gpt_oss_20B_GRPO/README.md)
* [TinyQwen3 MoE](TinyQwen3_MoE/README.md)
* [Meta Synthetic Data Llama3 2 (3B)](Meta_Synthetic_Data_Llama3_2_3B/README.md)
* [ModernBert](ModernBert/README.md)
* [Nemotron-3-Nano-30B-A3B A100](Nemotron_3_Nano_30B_A3B_A100/README.md)
* [Oute TTS (1B)](Oute_TTS_1B/README.md)
* [Orpheus (3B)-TTS](Orpheus_3B_TTS/README.md)
* [Phi 4-Conversational](Phi_4_Conversational/README.md)
* [Qwen3 (0 6B)-Phone Deployment](Qwen3_0_6B_Phone_Deployment/README.md)
* [Qwen3 (14B)-Reasoning-Conversational](Qwen3_14B_Reasoning_Conversational/README.md)
* [Qwen3 (4B) Instruct-QAT](Qwen3_4B_Instruct_QAT/README.md)
* [Qwen3 8B FP8 GRPO](Qwen3_8B_FP8_GRPO/README.md)
* [Qwen3 MoE](Qwen3_MoE/README.md)
* [Spark TTS (0 5B)](Spark_TTS_0_5B/README.md)
* [bert classification](bert_classification/README.md)
* [Goal: Make faster kernels with Reinforcement Learning](gpt_oss_20B_GRPO_BF16/README.md)

## 🛤️ Moving to Production & Real-World Projects
To transition these implementations from local notebooks to production environments:
1. **Model Export**: Use Unsloth's `model.save_pretrained_gguf` or `model.save_pretrained_merged` for deployment via vLLM or Ollama.
2. **Quantization**: Strategically apply 4-bit, FP8, or GGUF quantization based on the target inference hardware (Cloud vs Edge).
3. **Continuous Integration**: Automate evaluation runs using the provided benchmarks to ensure quality before deployment.
4. **Monitoring**: Integrate with tools like Weights & Biases for real-time tracking of fine-tuning runs.
