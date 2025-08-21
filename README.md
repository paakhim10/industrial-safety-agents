# Visual Agents for Industrial Safety (VLM Research)

This repository documents research and development conducted on **Vision-Language Models (VLMs)** for industrial safety and compliance monitoring. The goal is to evaluate and prototype **visual agents** that extend beyond traditional object detection pipelines by enabling **semantic understanding**, **real-time reasoning**, and **natural language interaction** for safety-critical environments.

### Background & Motivation

Earlier implementations in this space relied on **YOLOX** integrated with **DLStreamer pipelines** for structured object detection and alerting. While these pipelines achieved reliable detection performance, they lacked the semantic reasoning and open-ended query handling needed for more adaptive safety systems. Specifically, they were limited in:

* **Temporal reasoning** (understanding actions/events across frames)
* **Spatial awareness** (relationships between entities in context)
* **Flexibility and extensibility** (adapting to new rules/queries)
* **Real-time user interaction** (dynamic queries from safety operators)

With **visual AI agents**, these drawbacks can be mitigated. This repository extends that line of work by investigating **VLM-based visual agents**, combining detection with **language-guided understanding** to support **flexible compliance monitoring** in dynamic industrial environments.

### Repository Contents

* **Reports** – Documented testing results of VLMs on industrial safety datasets and real-time scenarios.
* **Notebooks** – Demo notebooks running VLMs on sample safety tasks (image-based and video-based).
* **Demos** – Real-world implementations such as interactive web-based VQA/captioning pages for safety monitoring.

### Current Focus

* Benchmarking lightweight VLMs (e.g., SmolVLM, Florence-2, LLaVA-OneVision, Flash-VStream) for **streaming video safety analysis**.
* Fine-tuning light (< 1 billion parameters) and heavy (> 2 billion parameters) VLMs on industrial safety use cases.
* Exploring integration of **temporal + spatial reasoning** into monitoring workflows.

### Next Steps
* **Streaming & Low-Latency VLMs**
  Explore ReKV-enhanced StreamingVQA and Flash-VStream for near real-time deployments on edge devices.
* **Efficiency-Accuracy Tradeoffs**
  Benchmark SmolVLM and other compact architectures for deployment feasibility vs. heavier baselines (e.g., BLIP-2, Florence-2).
* **Domain Adaptation**
  Fine-tuning or instruction adaptation of open-source VLMs on industrial safety-specific corpora for better compliance detection.
* **Evaluation Framework**
  Standardize metrics for safety compliance QA (precision/recall on safety violations, latency benchmarks, qualitative failure case logging).
* **Deployment Prototypes**
  Extend real-world demos with integrated backend APIs for processing continuous video streams, mimicking real industrial monitoring setups.

