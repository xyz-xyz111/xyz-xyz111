# Hi, I'm Qisheng Shi 👋

Data Science master's student at Nankai University, focused on **LLM agents, RAG, instruction-data synthesis, and post-training alignment**. I design and build end-to-end training and evaluation pipelines from research ideas.

目前专注于大模型应用与训练工程，正在寻找 **AI / LLM 算法实习机会**。

📄 [下载中文简历](./resume/28石奇生南开大学数据科学研一可立即到岗实习6个月以上.pdf)

## Featured projects

### [NanoRAFT-RL](https://github.com/xyz-xyz111/NanoRAFT-RL)

Single-GPU implementation of retrieval-augmented fine-tuning and PPO alignment on Qwen2-7B.

- Engineering focus: stable PPO training and configurable evaluation on one RTX 4090
- Fixed TRL 0.7.4's PEFT reference-policy path by explicitly loading and freezing the SFT reference model
- Added conservative PPO controls, length-aware rewards, high-KL early stopping, parameter checks, and CLI evaluation options
- Result: PPO reached **0.826** versus **0.360** for Base (`+129.4%`), with observed KL around `-0.6–0.6`

`PyTorch` `Transformers` `PEFT` `QLoRA` `TRL` `PPO` `RAFT`

### [MLangChain](https://github.com/xyz-xyz111/MLangChain)

LangGraph-based multi-agent pipeline for generating and refining Alpaca-format instruction data.

- Engineering focus: heterogeneous LLM feedback normalization and end-to-end workflow validation
- Added Pydantic-compatible handling for string, dictionary, list, and nested Critic feedback
- Preserved structured `location / problem / suggestion` information for targeted refinement
- Result: **9.5/10** after 2 iterations, with **10/10 facts verified and 0 contradictions**

`Python` `LangGraph` `LangChain` `RAG` `Pydantic` `Tavily`

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
