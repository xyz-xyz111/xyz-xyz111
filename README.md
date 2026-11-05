# Hi, I'm Qisheng Shi 👋

Data Science master's student at Nankai University, focused on **LLM agents, RAG, instruction-data synthesis, and post-training alignment**. I design and build end-to-end training and evaluation pipelines from research ideas.

目前专注于大模型应用与训练工程，正在寻找 **AI / LLM 算法实习机会**。

## Featured projects

### [MLangChain](https://github.com/xyz-xyz111/MLangChain)

LangGraph-based multi-agent pipeline for generating and refining Alpaca-format instruction data.

- Coordinates **Generator → Critic → Refiner** agents through shared state
- Uses task-aware grading for code, reasoning, explanation, and creative tasks
- Adds Tavily-based RAG fact checking and structured revision feedback
- Adds Best-of-N comparison, rollback control, complexity evolution, and Pydantic-compatible feedback normalization
- Result: average quality **8.83 → 9.10**, scoring variance **±1.0 → ±0.2**, factual accuracy **85% → 95%**

`Python` `LangGraph` `LangChain` `RAG` `Pydantic` `Tavily`

### [NanoRAFT-RL](https://github.com/xyz-xyz111/NanoRAFT-RL)

Single-GPU implementation of retrieval-augmented fine-tuning and PPO alignment on Qwen2-7B.

- Built a complete **RAFT-SFT → PPO → unified evaluation** pipeline on one RTX 4090
- Fixed TRL 0.7.4's PEFT reference-policy path by explicitly loading and freezing the SFT reference model
- Added conservative PPO controls, length-aware rewards, high-KL early stopping, parameter checks, and configurable evaluation
- Result: RAFT-SFT reached **0.856** and PPO reached **0.779**, versus **0.360** for Base

`PyTorch` `Transformers` `PEFT` `QLoRA` `TRL` `PPO` `RAFT`

## Technical interests

- LLM agents and workflow orchestration
- Retrieval-augmented generation and evidence-grounded evaluation
- Instruction-data synthesis and quality control
- Parameter-efficient fine-tuning and reinforcement learning alignment
- Experiment design, debugging, and model evaluation

## Current focus

- Improving reward design with answer-correctness and evidence-consistency signals
- Expanding evaluations across larger test sets and multiple random seeds
- Building production-oriented LLM systems with measurable quality and reliability
