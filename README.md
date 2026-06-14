# Awesome Multimodal Agentic Frameworks

> A curated and continuously updated collection of papers, codebases, benchmarks, datasets, demos, tutorials, and applications for **Multimodal Agentic Systems**.
>
> Based on our TMLR survey: *"A Survey on Foundations and Frontiers of Multimodal Agentic Frameworks: Techniques and Applications"*.

[![Paper](https://img.shields.io/badge/TMLR-Paper-red)]()
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Contributions Welcome](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)]()
[![License](https://img.shields.io/badge/License-MIT-blue.svg)]()

---

## 📢 News

* **Ongoing:** Actively accepting community contributions.
* **June 2026:** Repository launched.
* **May 2026:** Our survey paper was accepted at TMLR.

---

# Overview

Recent advances in Large Language Models (LLMs) and Large Multimodal Models (LMMs) have enabled the emergence of **agentic systems** capable of perceiving, reasoning, remembering, planning, and acting in complex environments.

Unlike traditional LLM agents that rely heavily on textual abstractions, modern multimodal agents operate directly on images, video, audio, GUI screenshots, web interfaces, and physical environments.

This repository extends our survey into a **living resource** that organizes:

* 📄 Research papers
* 💻 Open-source implementations
* 🎥 Demos and project pages
* 📊 Benchmarks and leaderboards
* 📚 Tutorials and educational resources
* 🚀 Industrial applications

---

# What is a Multimodal Agent?

We define a multimodal agent as:

> An agentic framework that uses a Large Multimodal Model (LMM) to perceive, reason, plan, and act across multiple modalities simultaneously.

Unlike text-only agents, multimodal agents can directly leverage:

* Images
* Video
* Audio
* GUI Screens
* Web Interfaces
* Sensor Streams
* Physical Environments

---

# Taxonomy

Our survey organizes multimodal agents around the cognitive loop:

```text
Perceive → Reason → Remember → Plan → Act
```

---

## 1. Perception

### Delegated Perception

Tool-calling systems that convert modalities into text.

Examples:

* HuggingGPT
* Visual ChatGPT
* MM-ReAct
* VisProg

📚 TODO: Papers will go there

---

### Late-Fusion Perception

Separate modality encoders project information into an LLM embedding space.

Examples:

* Flamingo
* LLaVA
* LLaVA-Plus
* PaLM-E
* RT-2
* OpenVLA

📚 TODO: Papers will go there

---

### Early-Fusion Perception

Native multimodal processing through unified architectures.

Examples:

* GPT-4o
* Gemini 1.5
* Chameleon
* Fuyu
* Janus-Pro

📚 TODO: Papers will go there

---

## 2. Reasoning & Planning

### Language-Based Reasoning

* Chain-of-Thought
* Tree-of-Thought
* ReAct
* Reflexion

### Visually Grounded Reasoning

* SeeAct
* WebVoyager
* Magma
* RT-2

### Cross-Modal Reasoning

* PandaGPT
* NExT-GPT
* CoDi-2
* ReelWave

📚 TODO: Papers will go there

---

## 3. Memory

### Modality-Specific Memory

* HuggingGPT
* Visual ChatGPT
* VideoAgent

### Unified Memory

* GPT-4o
* Gemini
* HMRAG

### Long-Horizon Memory

* Reflexion
* AppAgent-v2
* GUI-Owl

📚 TODO: Papers will go there

---

## 4. Action

### Language-Driven Actions

* ToolFormer
* Gorilla
* ToolLLM

### Visually Grounded Actions

* AppAgent
* CogAgent
* WebVoyager
* Mobile-Agent

### Embodied Actions

* SayCan
* RT-2
* OpenVLA
* PaLM-E

📚 TODO: Papers will go there

---

# Papers by Application Domain

---

## 🤖 Robotics & Physical Embodiment

### Surveys

| Paper        | Year | Code |
| ------------ | ---- | ---- |
| Survey Paper | 2026 | Link |

### Foundation Models

* RT-2
* OpenVLA
* PaLM-E
* Magma
* SayCan

### Benchmarks

* CALVIN
* BridgeData
* LIBERO

📚 TODO: Papers will go there

---

## 🌐 GUI & Web Navigation

### Web Agents

* WebGPT
* WebVoyager
* BrowserGym Agents

### Mobile Agents

* AppAgent
* Mobile-Agent
* AutoDroid

### Desktop Agents

* CogAgent
* Ferret-UI
* SeeAct

📚 TODO: Papers will go there

---

## 🎨 Multimedia Content Generation & Editing

### Image Editing

* InstructPix2Pix
* LLaVA-Plus
* Visual ChatGPT

### Video Editing

* VideoComposer
* VideoDirectorGPT

### Audio Editing

* WavCraft
* WavJourney

📚 TODO: Papers will go there

---

## 🎥 Long-Form Video Understanding & Retrieval

### Retrieval-Based Systems

* VideoAgent
* VLog

### Video Reasoning

* VideoMind
* LVAgent
* Vgent

📚 TODO: Papers will go there

---

# Benchmarks

| Benchmark    | Domain             | Modality | Metric          |
| ------------ | ------------------ | -------- | --------------- |
| WebArena     | Web Navigation     | GUI      | Success Rate    |
| AndroidWorld | Mobile Agents      | GUI      | Task Completion |
| EgoSchema    | Long Video         | Video    | Accuracy        |
| MMVet        | Multimodal QA      | Image    | Score           |
| MMMU         | General Multimodal | Multi    | Accuracy        |

📚 TODO: List of benchmarks go there

---

# Open-Source Projects

## General Agent Frameworks

| Project  | Stars | Code |
| -------- | ----- | ---- |
| OpenVLA  | ⭐     | Link |
| CogAgent | ⭐     | Link |
| AppAgent | ⭐     | Link |

---

## Libraries

* LangGraph
* AutoGen
* CrewAI
* OpenAI Agents SDK
* Haystack

---

# Datasets

## Robotics

* BridgeData
* RT-X

## GUI Navigation

* Mind2Web
* AndroidControl
* WebArena

## Long Video

* EgoSchema
* Video-MME

## Multimedia Editing

* Pico-Banana-400K
* EditBench

📚 TODO: List of datasets go here

---

# Tutorials & Learning Resources

## Beginner

* Introduction to LLM Agents
* Introduction to Multimodal Learning
* Agent Design Patterns

## Intermediate

* Building Web Agents
* Building GUI Agents
* Retrieval-Augmented Agents

## Advanced

* Vision-Language-Action Models
* Agent Memory Systems
* Multimodal Planning

---

# Industrial Systems

## Robotics

* Figure AI
* Covariant
* Physical Intelligence

## GUI Agents

* OpenAI Operator
* Anthropic Computer Use

## Productivity Agents

* Devin
* Manus

---

# Leaderboards

| Category            | Leaderboard |
| ------------------- | ----------- |
| Web Agents          | Link        |
| GUI Agents          | Link        |
| Robotics            | Link        |
| Video Understanding | Link        |

---

# Research Trends

## 2023

* Tool Calling
* ReAct
* Visual Tool Use

## 2024

* Vision-Language-Action Models
* GUI Agents
* Long Context Video Agents

## 2025

* Native Multimodal Agents
* Unified Memory
* Cross-Modal Planning

## 2026+

* Agent Operating Systems
* Generalist Embodied Agents
* Long-Horizon Autonomous Systems

---

# Contribution Guide

We welcome contributions from researchers, students, and practitioners.

## What can be contributed?

### Papers

Please include:

```yaml
Title:
Authors:
Venue:
Year:
Domain:
Modality:
Fusion Strategy:
Code:
Project Page:
```

### Repositories

### Datasets

### Benchmarks

### Tutorials

### Industry Applications

---

## Adding a Paper

Create a pull request with the following format:

```markdown
- [Paper Title](link)
  - Venue: NeurIPS 2026
  - Code: link
  - Domain: GUI Navigation
  - Fusion: Early-Fusion
```

---

# Repository Structure

```text
awesome-multimodal-agents
│
├── papers
│   ├── perception
│   ├── reasoning
│   ├── memory
│   └── action
│
├── domains
│   ├── robotics
│   ├── gui_web
│   ├── multimedia
│   └── long_video
│
├── datasets
├── benchmarks
├── tutorials
├── applications
└── assets
```

---

# Citation

If you find this repository useful, please cite:

```bibtex
@article{mokaria2026a,
title={A Survey on Foundations and Frontiers of Multimodal Agentic Frameworks: Techniques and Applications},
author={Neel Mokaria and Rishie Raj and Dheeraj Baiju and Xiaoqian Shen and Shraman Pramanick and Kevin Qinghong Lin and Arda Senocak and Mike Zheng Shou and Philip Torr and Mohamed Elhoseiny and Yapeng Tian and Ruohan Gao and Salman Khan and Sayan Nag and Sanjoy Chowdhury and Dinesh Manocha},
journal={Transactions on Machine Learning Research},
issn={2835-8856},
year={2026},
url={https://openreview.net/forum?id=eaVoaI7f8v},
note={}
}
```

---

# Acknowledgements

This repository is maintained by the authors of:

**A Survey on Foundations and Frontiers of Multimodal Agentic Frameworks**

and the broader multimodal AI research community.

---

# License

MIT License

---


