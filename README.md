# Hi, I'm Qisheng Shi 👋

Data Science master's student at Nankai University, focused on **LLM agents, RAG, instruction-data synthesis, and post-training alignment**. I enjoy turning research ideas into reproducible training and evaluation pipelines.

目前专注于大模型应用与训练工程，正在寻找 **AI / LLM 算法实习机会**。

## Featured projects

### [MLangChain](https://github.com/xyz-xyz111/MLangChain)

LangGraph-based multi-agent pipeline for generating and refining Alpaca-format instruction data.

- Coordinates **Generator → Critic → Refiner** agents through shared state
- Uses task-aware grading for code, reasoning, explanation, and creative tasks
- Adds Tavily-based RAG fact checking and structured revision feedback
- End-to-end result: **9.5/10**, 2 refinement iterations, **10 verified facts with 0 contradictions**
- Fixed heterogeneous LLM feedback parsing with Pydantic-compatible normalization

`Python` `LangGraph` `LangChain` `RAG` `Pydantic` `Tavily`

### [NanoRAFT-RL](https://github.com/xyz-xyz111/NanoRAFT-RL)

Single-GPU reproduction of retrieval-augmented fine-tuning and PPO alignment on Qwen2-7B.

- Builds RAFT samples with relevant evidence and distractor documents
- Runs a complete **RAFT-SFT → PPO → unified evaluation** pipeline on one RTX 4090
- RAFT-SFT score: **0.360 → 0.838** (`+132.8%` over Base)
- Diagnosed TRL 0.7.4's PEFT reference-policy issue and reduced KL from roughly **30–135 to -0.6–0.6**
- Improved PPO score from **0.410 to 0.826**, while reducing average response length from **1001 to 614**

`PyTorch` `Transformers` `PEFT` `QLoRA` `TRL` `PPO` `RAFT`

## Technical interests

- LLM agents and workflow orchestration
- Retrieval-augmented generation and evidence-grounded evaluation
- Instruction-data synthesis and quality control
- Parameter-efficient fine-tuning and reinforcement learning alignment
- Reproducible experiments, debugging, and model evaluation

## Current focus

- Improving reward design with answer-correctness and evidence-consistency signals
- Expanding evaluations across larger test sets and multiple random seeds
- Building production-oriented LLM systems with measurable quality and reliability
