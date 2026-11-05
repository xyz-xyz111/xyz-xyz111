# Hi, I'm Qisheng Shi 👋

Data Science master's student at Nankai University, focused on **LLM agents, RAG, instruction-data synthesis, and post-training alignment**. I design and build end-to-end training and evaluation pipelines from research ideas.

目前专注于大模型应用与训练工程，正在寻找 **AI / LLM 算法实习机会**。

## Featured projects

### [MLangChain](https://github.com/xyz-xyz111/MLangChain)

LangGraph-based multi-agent pipeline for generating and refining Alpaca-format instruction data.

- Connected the **Generator → Critic → Refiner** workflow with Tavily-based fact checking
- Fixed heterogeneous LLM feedback parsing with Pydantic-compatible state normalization
- Preserved structured `location / problem / suggestion` feedback for targeted revisions
- Result: **9.5/10** after 2 refinement iterations, with **10/10 facts verified and 0 contradictions**

`Python` `LangGraph` `LangChain` `RAG` `Pydantic` `Tavily`

### [NanoRAFT-RL](https://github.com/xyz-xyz111/NanoRAFT-RL)

Single-GPU implementation of retrieval-augmented fine-tuning and PPO alignment on Qwen2-7B.

- Implemented RAFT data construction with relevant evidence and distractor documents
- Built a 4-bit **RAFT-SFT → PPO → unified evaluation** pipeline for one RTX 4090
- Fixed TRL 0.7.4's PEFT reference-policy path and kept observed KL near zero (`-0.6–0.6`)
- Result: RAFT-SFT reached **0.838** and PPO reached **0.826**, versus **0.360** for Base

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
