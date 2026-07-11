# Awesome Multimodal Agentic Frameworks

> A curated and continuously updated collection of papers, codebases, benchmarks, datasets, demos, tutorials, and applications for **Multimodal Agentic Systems**.
>
> Based on our TMLR survey: *"A Survey on Foundations and Frontiers of Multimodal Agentic Frameworks: Techniques and Applications"*.

[![Paper](https://img.shields.io/badge/TMLR-Paper-red)](https://openreview.net/forum?id=eaVoaI7f8v)
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

Each entry below links to the corresponding paper. Framework names are shown after the paper title when the title alone is not sufficiently descriptive.

## 1. Perception

### Delegated Perception

Tool-calling systems use specialist models to translate non-text modalities into representations a language-model orchestrator can consume.

* [HuggingGPT: Solving AI Tasks with ChatGPT and its Friends in Hugging Face](https://arxiv.org/abs/2303.17580) (2023)
* [Visual ChatGPT: Talking, Drawing and Editing with Visual Foundation Models](https://arxiv.org/abs/2303.04671) (2023)
* [MM-REACT: Prompting ChatGPT for Multimodal Reasoning and Action](https://arxiv.org/abs/2303.11381) (2023)
* [Visual Programming: Compositional Visual Reasoning without Training](https://arxiv.org/abs/2211.11559) — VISPROG (2022)
* [CLOVA: A Closed-Loop Visual Assistant with Tool Usage and Update](https://arxiv.org/abs/2312.10908) (2024)
* [Chameleon: Plug-and-Play Compositional Reasoning with Large Language Models](https://arxiv.org/abs/2304.09842) (2023)

### Late-Fusion Perception

Modality-specific encoders and projectors map sensory inputs into a language-model embedding space.

* [Flamingo: A Visual Language Model for Few-Shot Learning](https://arxiv.org/abs/2204.14198) (2022)
* [EgoVLP: Egocentric Video-Language Pre-training](https://arxiv.org/abs/2112.12169) (2022)
* [EgoVLPv2: Egocentric Video-Language Pre-training with Fusion in the Backbone](https://arxiv.org/abs/2307.05463) (2023)
* [Visual Instruction Tuning](https://arxiv.org/abs/2304.08485) — LLaVA (2023)
* [LLaVA-Plus: Learning to Use Tools for Creating Multimodal Agents](https://arxiv.org/abs/2401.05651) (2024)
* [Magma: A Foundation Model for Multimodal AI Agents](https://arxiv.org/abs/2502.13130) (2025)
* [LongVLM: Efficient Long Video Understanding via Large Language Models](https://arxiv.org/abs/2404.03384) (2024)
* [Video-XL: Extra-Long Vision Language Model for Hour-Scale Video Understanding](https://arxiv.org/abs/2409.14485) (2024)
* [MovieChat: From Dense Token to Sparse Memory for Long Video Understanding](https://arxiv.org/abs/2307.16449) (2024)
* [RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control](https://arxiv.org/abs/2307.15818) (2023)
* [OpenVLA: An Open-Source Vision-Language-Action Model](https://arxiv.org/abs/2406.09246) (2024)
* [PaLM-E: An Embodied Multimodal Language Model](https://arxiv.org/abs/2303.03378) (2023)
* [From Pixels to UI Actions: Learning to Follow Instructions via Graphical User Interfaces](https://arxiv.org/abs/2306.00245) — Pix2Act (2023)
* [Multimodal Web Navigation with Instruction-Finetuned Foundation Models](https://arxiv.org/abs/2305.11854) — WebGUM (2023)
* [CogAgent: A Visual Language Model for GUI Agents](https://arxiv.org/abs/2312.08914) (2024)
* [Ferret-UI: Grounded Mobile UI Understanding with Multimodal LLMs](https://arxiv.org/abs/2404.05719) (2024)

### Early-Fusion Perception

Unified architectures process multiple modalities natively in a shared model.

* [GPT-4o System Card](https://arxiv.org/abs/2410.21276) (2024)
* [Gemini 1.5: Unlocking Multimodal Understanding across Millions of Tokens of Context](https://arxiv.org/abs/2403.05530) (2024)
* [Chameleon: Mixed-Modal Early-Fusion Foundation Models](https://arxiv.org/abs/2405.09818) (2024)
* [Fuyu-8B](https://www.adept.ai/blog/fuyu-8b) — model release (2023)
* [LongVILA: Scaling Long-Context Visual Language Models for Long Videos](https://arxiv.org/abs/2408.10188) (2024)
* [Transfusion: Predict the Next Token and Diffuse Images with One Multi-Modal Model](https://arxiv.org/abs/2408.11039) (2024)
* [Show-o: One Single Transformer to Unify Multimodal Understanding and Generation](https://arxiv.org/abs/2408.12528) (2024)
* [Janus-Pro: Unified Multimodal Understanding and Generation with Data and Model Scaling](https://arxiv.org/abs/2501.17811) (2025)

## 2. Reasoning & Planning

### Language-Based Reasoning

* [Chain-of-Thought Prompting Elicits Reasoning in Large Language Models](https://arxiv.org/abs/2201.11903) (2022)
* [Tree of Thoughts: Deliberate Problem Solving with Large Language Models](https://arxiv.org/abs/2305.10601) (2023)
* [ReAct: Synergizing Reasoning and Acting in Language Models](https://arxiv.org/abs/2210.03629) (2022)
* [Reflexion: Language Agents with Verbal Reinforcement Learning](https://arxiv.org/abs/2303.11366) (2023)

### Visually Grounded Reasoning

* [GPT-4V(ision) is a Generalist Web Agent, if Grounded](https://arxiv.org/abs/2401.01614) — SeeAct (2024)
* [WebVoyager: Building an End-to-End Web Agent with Large Multimodal Models](https://arxiv.org/abs/2401.13919) (2024)
* [Magma: A Foundation Model for Multimodal AI Agents](https://arxiv.org/abs/2502.13130) (2025)
* [RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control](https://arxiv.org/abs/2307.15818) (2023)
* [OpenVLA: An Open-Source Vision-Language-Action Model](https://arxiv.org/abs/2406.09246) (2024)
* [VideoAgent: Long-form Video Understanding with Large Language Model as Agent](https://arxiv.org/abs/2403.10517) (2024)

### Cross-Modal Reasoning

* [ImageBind: One Embedding Space to Bind Them All](https://arxiv.org/abs/2305.05665) (2023)
* [PandaGPT: One Model to Instruction-Follow Them All](https://arxiv.org/abs/2305.16355) (2023)
* [NExT-GPT: Any-to-Any Multimodal LLM](https://arxiv.org/abs/2309.05519) (2024)
* [CoDi-2: In-Context Interleaved and Interactive Any-to-Any Generation](https://arxiv.org/abs/2311.18775) (2024)
* [ReelWave: Multi-Agentic Movie Sound Generation through Multimodal LLM Conversation](https://arxiv.org/abs/2503.07217) (2025)
* [AudioAgent: Enhancing Task Performance through Modality-Driven Prompt Optimization](https://openreview.net/forum?id=VLzLj7dU9b) (2024)

## 3. Memory

### Modality-Specific Memory

* [HuggingGPT: Solving AI Tasks with ChatGPT and its Friends in Hugging Face](https://arxiv.org/abs/2303.17580) (2023)
* [Visual ChatGPT: Talking, Drawing and Editing with Visual Foundation Models](https://arxiv.org/abs/2303.04671) (2023)
* [VideoAgent: Long-form Video Understanding with Large Language Model as Agent](https://arxiv.org/abs/2403.10517) (2024)

### Unified Memory

* [Gemini 1.5: Unlocking Multimodal Understanding across Millions of Tokens of Context](https://arxiv.org/abs/2403.05530) (2024)
* [GPT-4o System Card](https://arxiv.org/abs/2410.21276) (2024)
* [HM-RAG: Hierarchical Multi-Agent Multimodal Retrieval Augmented Generation](https://arxiv.org/abs/2503.06789) (2025)
* [ImageBind: One Embedding Space to Bind Them All](https://arxiv.org/abs/2305.05665) (2023)
* [SonicRAG: High Fidelity Sound Effects Synthesis Based on Retrieval Augmented Generation](https://arxiv.org/abs/2505.03244) (2025)

### Temporal Context Management

* [Mobile-Agent-v2: Mobile Device Operation Assistant with Effective Navigation via Multi-Agent Collaboration](https://arxiv.org/abs/2406.01014) (2024)
* [AppAgent v2: Advanced Agent for Flexible Mobile Interactions](https://arxiv.org/abs/2408.11824) (2024)
* [Reflexion: Language Agents with Verbal Reinforcement Learning](https://arxiv.org/abs/2303.11366) (2023)
* [Mobile-Agent-v3: Fundamental Agents for GUI Automation](https://arxiv.org/abs/2508.15144) (2025)

### Bandwidth Management

* [VideoAgent: A Memory-augmented Multimodal Agent for Video Understanding](https://arxiv.org/abs/2403.11481) (2024)
* [A Simple LLM Framework for Long-Range Video Question-Answering](https://arxiv.org/abs/2312.17235) — LLoVi (2024)
* [DoraemonGPT: Toward Understanding Dynamic Scenes with Large Language Models](https://arxiv.org/abs/2501.01234) (2025)

## 4. Action

### Language-Driven Actions

* [Toolformer: Language Models Can Teach Themselves to Use Tools](https://arxiv.org/abs/2302.04761) (2023)
* [Gorilla: Large Language Model Connected with Massive APIs](https://arxiv.org/abs/2305.15334) (2023)
* [MLLM-Tool: A Multimodal Large Language Model for Tool Agent Learning](https://arxiv.org/abs/2502.02345) (2025)
* [ToolLLM: Facilitating Large Language Models to Master 16,000+ Real-World APIs](https://arxiv.org/abs/2307.16789) (2023)

### Visually Grounded Actions

* [AppAgent: Multimodal Agents as Smartphone Users](https://arxiv.org/abs/2312.13771) (2023)
* [CogAgent: A Visual Language Model for GUI Agents](https://arxiv.org/abs/2312.08914) (2024)
* [WebVoyager: Building an End-to-End Web Agent with Large Multimodal Models](https://arxiv.org/abs/2401.13919) (2024)
* [Mobile-Agent: Autonomous Multi-Modal Mobile Device Agent with Visual Perception](https://arxiv.org/abs/2401.16158) (2024)
* [VoxPoser: Composable 3D Value Maps for Robotic Manipulation with Language Models](https://arxiv.org/abs/2307.05973) (2023)

### Embodied Multimodal Actions

* [Do As I Can, Not As I Say: Grounding Language in Robotic Affordances](https://arxiv.org/abs/2204.01691) — SayCan (2022)
* [RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control](https://arxiv.org/abs/2307.15818) (2023)
* [OpenVLA: An Open-Source Vision-Language-Action Model](https://arxiv.org/abs/2406.09246) (2024)
* [PaLM-E: An Embodied Multimodal Language Model](https://arxiv.org/abs/2303.03378) (2023)
* [Octo: An Open-Source Generalist Robot Policy](https://arxiv.org/abs/2405.12213) (2024)

# Papers by Application Domain

## 🤖 Robotics & Physical Embodiment

### Language-Grounded Planning and Control

* [Do As I Can, Not As I Say: Grounding Language in Robotic Affordances](https://arxiv.org/abs/2204.01691) — SayCan (2022)
* [Inner Monologue: Embodied Reasoning through Planning with Language Models](https://arxiv.org/abs/2207.05608) (2022)
* [Code as Policies: Language Model Programs for Embodied Control](https://arxiv.org/abs/2209.07753) (2023)
* [Look Before You Leap: Unveiling the Power of GPT-4V in Robotic Vision-Language Planning](https://arxiv.org/abs/2311.17842) (2023)

### Vision-Language-Action Models

* [PaLM-E: An Embodied Multimodal Language Model](https://arxiv.org/abs/2303.03378) (2023)
* [RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control](https://arxiv.org/abs/2307.15818) (2023)
* [Octo: An Open-Source Generalist Robot Policy](https://arxiv.org/abs/2405.12213) (2024)
* [OpenVLA: An Open-Source Vision-Language-Action Model](https://arxiv.org/abs/2406.09246) (2024)
* [Magma: A Foundation Model for Multimodal AI Agents](https://arxiv.org/abs/2502.13130) (2025)
* [$\pi_0$: A Vision-Language-Action Flow Model for General Robot Control](https://arxiv.org/abs/2410.24164) (2024)
* [GR00T N1: An Open Foundation Model for Generalist Humanoid Robots](https://arxiv.org/abs/2503.14734) (2025)

### Multi-Robot Systems

* [RoCo: Dialectic Multi-Robot Collaboration with Large Language Models](https://arxiv.org/abs/2307.04738) (2024)
* [Co-NavGPT: Multi-Robot Cooperative Visual Semantic Navigation using Large Language Models](https://arxiv.org/abs/2310.07937) (2023)
* [SMART-LLM: Smart Multi-Agent Robot Task Planning using Large Language Models](https://arxiv.org/abs/2309.10062) (2024)

## 🌐 GUI & Web Navigation

### Text and DOM-Based Agents

* [WebGPT: Browser-Assisted Question-Answering with Human Feedback](https://arxiv.org/abs/2112.09332) (2021)
* [WebGLM: Towards an Efficient Web-Enhanced Question Answering System with Human Preferences](https://arxiv.org/abs/2306.07906) (2023)
* [A Real-World WebAgent with Planning, Long Context Understanding, and Program Synthesis](https://arxiv.org/abs/2307.12856) (2023)
* [AutoDroid: LLM-Powered Task Automation in Android](https://arxiv.org/abs/2308.15272) (2024)
* [AssistGUI: Task-Oriented Desktop Graphical User Interface Automation](https://arxiv.org/abs/2312.13108) (2023)
* [AutoWebGLM: A Large Language Model-Based Web Navigating Agent](https://arxiv.org/abs/2404.03648) (2024)

### Fine-Tuned Multimodal Agents

* [Multimodal Web Navigation with Instruction-Finetuned Foundation Models](https://arxiv.org/abs/2305.11854) — WebGUM (2023)
* [From Pixels to UI Actions: Learning to Follow Instructions via Graphical User Interfaces](https://arxiv.org/abs/2306.00245) — Pix2Act (2023)
* [CogAgent: A Visual Language Model for GUI Agents](https://arxiv.org/abs/2312.08914) (2024)
* [Ferret-UI: Grounded Mobile UI Understanding with Multimodal LLMs](https://arxiv.org/abs/2404.05719) (2024)
* [SeeClick: Harnessing GUI Grounding for Advanced Visual GUI Agents](https://arxiv.org/abs/2401.10935) (2024)
* [ShowUI: One Vision-Language-Action Model for GUI Visual Agent](https://arxiv.org/abs/2411.17465) (2025)

### Native and API-Based Multimodal Agents

* [GPT-4V(ision) is a Generalist Web Agent, if Grounded](https://arxiv.org/abs/2401.01614) — SeeAct (2024)
* [WebVoyager: Building an End-to-End Web Agent with Large Multimodal Models](https://arxiv.org/abs/2401.13919) (2024)
* [AppAgent: Multimodal Agents as Smartphone Users](https://arxiv.org/abs/2312.13771) (2023)
* [Mobile-Agent: Autonomous Multi-Modal Mobile Device Agent with Visual Perception](https://arxiv.org/abs/2401.16158) (2024)
* [GPT-4V in Wonderland: Large Multimodal Models for Zero-Shot Smartphone GUI Navigation](https://arxiv.org/abs/2311.07562) — MM-Navigator (2023)
* [Cradle: Empowering Foundation Agents towards General Computer Control](https://arxiv.org/abs/2403.03186) (2024)
* [Mobile-Agent-v2: Mobile Device Operation Assistant with Effective Navigation via Multi-Agent Collaboration](https://arxiv.org/abs/2406.01014) (2024)

## 🎨 Multimedia Content Generation & Editing

### Delegated Tool-Based Agents

* [Visual Programming: Compositional Visual Reasoning without Training](https://arxiv.org/abs/2211.11559) — VISPROG (2022)
* [AudioGPT: Understanding and Generating Speech, Music, Sound, and Talking Head](https://arxiv.org/abs/2304.12995) (2023)
* [WavJourney: Compositional Audio Creation with Large Language Models](https://arxiv.org/abs/2307.14335) (2023)
* [WavCraft: Audio Editing and Generation with Large Language Models](https://arxiv.org/abs/2403.09527) (2024)
* [LAVE: LLM-Powered Agent Assistance and Language Augmentation for Video Editing](https://arxiv.org/abs/2402.10294) (2024)
* [CLOVA: A Closed-Loop Visual Assistant with Tool Usage and Update](https://arxiv.org/abs/2312.10908) (2024)

### Native and Tuning-Free Agents

* [GenArtist: Multimodal LLM as an Agent for Unified Image Generation and Editing](https://arxiv.org/abs/2407.05600) (2024)
* [CoSTA*: Cost-Sensitive Toolpath Agent for Multi-Turn Image Editing](https://arxiv.org/abs/2503.10613) (2025)
* [FaSTA*: Fast-Slow Toolpath Agent with Subroutine Mining for Efficient Multi-Turn Image Editing](https://arxiv.org/abs/2506.20911) (2025)
* [FLATTEN: Optical Flow-Guided Attention for Consistent Text-to-Video Editing](https://arxiv.org/abs/2310.05922) (2023)
* [UniEdit: A Unified Tuning-Free Framework for Video Motion and Appearance Editing](https://arxiv.org/abs/2402.13185) (2025)
* [AnyV2V: A Tuning-Free Framework for Any Video-to-Video Editing Tasks](https://arxiv.org/abs/2403.14468) (2024)

### Multi-Agent Creative Systems

* [CREA: A Collaborative Multi-Agent Framework for Creative Image Editing and Generation](https://arxiv.org/abs/2504.05306) (2025)
* [ReelWave: Multi-Agentic Movie Sound Generation through Multimodal LLM Conversation](https://arxiv.org/abs/2503.07217) (2025)
* [Paper2Poster: Towards Multimodal Poster Automation from Scientific Papers](https://arxiv.org/abs/2505.21497) (2026)
* [Paper2Video: Automatic Video Generation from Scientific Papers](https://arxiv.org/abs/2510.05096) (2025)

## 🎥 Long-Form Video Understanding & Retrieval

### Iterative Retrieval Agents

* [AssistGPT: A General Multi-Modal Assistant that Can Plan, Execute, Inspect, and Learn](https://arxiv.org/abs/2306.08640) (2023)
* [VideoAgent: Long-form Video Understanding with Large Language Model as Agent](https://arxiv.org/abs/2403.10517) (2024)
* [A Simple LLM Framework for Long-Range Video Question-Answering](https://arxiv.org/abs/2312.17235) — LLoVi (2024)

### Specialized Fine-Tuned Agents

* [VideoMind: A Chain-of-LoRA Agent for Long Video Reasoning](https://arxiv.org/abs/2503.13444) (2025)
* [VLog: Video-Language Models by Generative Retrieval of Narration Vocabulary](https://arxiv.org/abs/2503.09402) (2025)

### Native and Agentic Long-Video Systems

* [DoraemonGPT: Toward Understanding Dynamic Scenes with Large Language Models](https://arxiv.org/abs/2501.01234) (2025)
* [VideoRAG: Retrieval-Augmented Generation with Extreme Long-Context Videos](https://arxiv.org/abs/2502.01549) (2025)
* [VideoDeepResearch: Long Video Understanding with Agentic Tool Using](https://arxiv.org/abs/2506.10821) (2025)
* [Deep Video Discovery: Agentic Search with Tool Use for Long-Form Video Understanding](https://arxiv.org/abs/2505.18079) (2025)

# Benchmarks

| Benchmark | Domain | Primary evaluation | Reference |
| --- | --- | --- | --- |
| CALVIN | Robotics | Long-horizon task success | [CALVIN: A Benchmark for Language-Conditioned Policy Learning](https://arxiv.org/abs/2112.03227) |
| LIBERO | Robotics | Lifelong manipulation task success | [LIBERO: Benchmarking Knowledge Transfer for Lifelong Robot Learning](https://arxiv.org/abs/2306.03310) |
| WebArena | Web navigation | Functional task success | [WebArena: A Realistic Web Environment for Building Autonomous Agents](https://arxiv.org/abs/2307.13854) |
| VisualWebArena | Visual web navigation | Functional task success | [VisualWebArena: Evaluating Multimodal Agents on Realistic Visual Web Tasks](https://arxiv.org/abs/2401.13649) |
| Mind2Web | Web navigation | Element and operation accuracy | [Mind2Web: Towards a Generalist Agent for the Web](https://arxiv.org/abs/2306.06070) |
| OSWorld | Computer use | End-to-end task success | [OSWorld: Benchmarking Multimodal Agents for Open-Ended Tasks](https://arxiv.org/abs/2404.07972) |
| EgoSchema | Long-form video | Multiple-choice accuracy | [EgoSchema: A Diagnostic Benchmark for Very Long-Form Video Language Understanding](https://arxiv.org/abs/2308.09126) |
| Video-MME | Long-form video | Multimodal QA accuracy | [Video-MME: The First-Ever Comprehensive Evaluation Benchmark of MLLMs in Video Analysis](https://arxiv.org/abs/2405.21075) |
| NExT-QA | Video reasoning | Causal and temporal QA accuracy | [NExT-QA: Next Phase of Question-Answering to Explaining Temporal Actions](https://arxiv.org/abs/2105.08276) |
| MagicBrush | Image editing | CLIP-based and human evaluation | [MagicBrush: A Manually Annotated Dataset for Instruction-Guided Image Editing](https://arxiv.org/abs/2306.10012) |
| GQA | Compositional visual reasoning | Question-answering accuracy | [GQA: A New Dataset for Real-World Visual Reasoning](https://arxiv.org/abs/1902.09506) |

# Open-Source Projects

| Project | Domain | Paper | Code |
| --- | --- | --- | --- |
| OpenVLA | Robotics | [Paper](https://arxiv.org/abs/2406.09246) | [GitHub](https://github.com/openvla/openvla) |
| Octo | Robotics | [Paper](https://arxiv.org/abs/2405.12213) | [GitHub](https://github.com/octo-models/octo) |
| Magma | General multimodal agents | [Paper](https://arxiv.org/abs/2502.13130) | [GitHub](https://github.com/microsoft/Magma) |
| CogAgent | GUI agents | [Paper](https://arxiv.org/abs/2312.08914) | [GitHub](https://github.com/THUDM/CogVLM) |
| SeeAct | Web agents | [Paper](https://arxiv.org/abs/2401.01614) | [GitHub](https://github.com/OSU-NLP-Group/SeeAct) |
| WebVoyager | Web agents | [Paper](https://arxiv.org/abs/2401.13919) | [GitHub](https://github.com/MinorJerry/WebVoyager) |
| AppAgent | Mobile agents | [Paper](https://arxiv.org/abs/2312.13771) | [GitHub](https://github.com/mnotgod96/AppAgent) |
| Mobile-Agent | Mobile agents | [Paper](https://arxiv.org/abs/2401.16158) | [GitHub](https://github.com/X-PLUG/MobileAgent) |
| VisualWebArena | GUI benchmark | [Paper](https://arxiv.org/abs/2401.13649) | [GitHub](https://github.com/web-arena-x/visualwebarena) |

# Datasets

The datasets below are used to train or evaluate frameworks discussed in the survey. Benchmark-style datasets are included here as data resources and in the benchmark table above as evaluation protocols.

## Robotics

* [BridgeData V2: A Dataset for Robot Learning at Scale](https://arxiv.org/abs/2308.12952) — [dataset](https://rail-berkeley.github.io/bridgedata/) (2023)
* [Open X-Embodiment: Robotic Learning Datasets and RT-X Models](https://arxiv.org/abs/2310.08864) — [dataset](https://robotics-transformer-x.github.io/) (2024)
* [GNM: A General Navigation Model to Drive Any Robot](https://arxiv.org/abs/2210.03370) — [dataset and code](https://github.com/robodhruv/visualnav-transformer) (2022)
* [CALVIN: A Benchmark for Language-Conditioned Policy Learning for Long-Horizon Robot Manipulation Tasks](https://arxiv.org/abs/2112.03227) — [dataset and code](https://github.com/mees/calvin) (2022)
* [LIBERO: Benchmarking Knowledge Transfer for Lifelong Robot Learning](https://arxiv.org/abs/2306.03310) — [dataset and code](https://github.com/Lifelong-Robot-Learning/LIBERO) (2023)

## GUI Navigation

* [Mind2Web: Towards a Generalist Agent for the Web](https://arxiv.org/abs/2306.06070) — [dataset](https://github.com/OSU-NLP-Group/Mind2Web) (2023)
* [WebArena: A Realistic Web Environment for Building Autonomous Agents](https://arxiv.org/abs/2307.13854) — [environment and data](https://github.com/web-arena-x/webarena) (2024)
* [VisualWebArena: Evaluating Multimodal Agents on Realistic Visual Web Tasks](https://arxiv.org/abs/2401.13649) — [environment and data](https://github.com/web-arena-x/visualwebarena) (2024)
* [Android in the Wild: A Large-Scale Dataset for Android Device Control](https://arxiv.org/abs/2307.10088) — [dataset](https://github.com/google-research/google-research/tree/master/android_in_the_wild) (2023)
* [OSWorld: Benchmarking Multimodal Agents for Open-Ended Tasks in Real Computer Environments](https://arxiv.org/abs/2404.07972) — [environment and data](https://github.com/xlang-ai/OSWorld) (2024)

## Long Video

* [EgoSchema: A Diagnostic Benchmark for Very Long-Form Video Language Understanding](https://arxiv.org/abs/2308.09126) — [dataset](https://egoschema.github.io/) (2023)
* [Video-MME: The First-Ever Comprehensive Evaluation Benchmark of MLLMs in Video Analysis](https://arxiv.org/abs/2405.21075) — [dataset](https://video-mme.github.io/home_page.html) (2024)
* [NExT-QA: Next Phase of Question-Answering to Explaining Temporal Actions](https://arxiv.org/abs/2105.08276) — [dataset](https://github.com/doc-doc/NExT-QA) (2021)

## Multimedia Editing

* [MagicBrush: A Manually Annotated Dataset for Instruction-Guided Image Editing](https://arxiv.org/abs/2306.10012) — [dataset](https://osu-nlp-group.github.io/MagicBrush/) (2023)
* [GQA: A New Dataset for Real-World Visual Reasoning and Compositional Question Answering](https://arxiv.org/abs/1902.09506) — [dataset](https://cs.stanford.edu/people/dorarad/gqa/) (2019)

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
├── README.md   # Taxonomy, domain papers, benchmarks, code, and datasets
└── LICENSE
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
