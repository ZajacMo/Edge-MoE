# Awesome Edge MoE: Optimization Strategies for LLMs on the Edge

<div align="center">
     <a href="#" target="_blank"><img src="https://img.shields.io/badge/Paper-Arxiv-red?logo=arxiv&style=flat-square" alt="arXiv"></a>
     <a href="https://github.com/ZajacMo/When-MoE-Meets-Edge"><img src="https://img.shields.io/github/stars/ZajacMo/When-MoE-Meets-Edge"/></a>
     <a href="https://github.com/ZajacMo/When-MoE-Meets-Edge"><img src="https://img.shields.io/github/forks/ZajacMo/When-MoE-Meets-Edge"/></a>
</div>

This repository provides a comprehensive collection of research papers, open-source projects, and optimization strategies for deploying **Mixture-of-Experts (MoE) Large Language Models on Edge Devices**. It includes contents from our survey paper 📖<em>"**Edge MoE: A Survey of Optimization Strategies for Mixture-of-Experts LLMs on the Edge**"</em> and will be continuously updated.

🤗 **You are very welcome to contribute to this repository** by launching an issue or a pull request. 

📫 **Contact us via emails:** `zhaoyong@uestc.edu.cn`

---



## 📜 Catalog

> **[Awesome Edge MoE](#awesome-edge-moe)**
>
> - **[🔥 News](#-news)**
> - **[📖 Overview](#-overview)**
>  - **[📚 Related Survey](#-survey)**
> - **[🪴 Taxonomy](#-taxonomy)**
>   - [System Optimization](#system-optimization)
>   - [Architecture Optimization](#architecture-optimization)
>   - [Parameter Optimization](#parameter-optimization)
> - **[🚀 Application Scenarios](#-application-scenarios)**
> - **[📃 Citation](#-citation)**

---

## 🔥 News

* **[2026-03]** 🔥🔥 Our survey on Edge MoE optimization strategies is released! 

## 📚 Related Survey Papers


## 🪴 Taxonomy

### System Optimization
#### Memory Management
##### Hierarchical Storage
- () **EdgeMoE: Empowering Sparse Large Language Models on Mobile Devices** [[paper]](https://doi.ieeecomputersociety.org/10.1109/TMC.2025.3546466)
- ()**Deep Learning and Machine Learning with GPGPU and CUDA: Unlocking the Power of Parallel Computing** [[paper]](https://arxiv.org/abs/2410.05686)
- ()
- ()
##### Expert Caching & Prefetching
- ()
- ()
- ()
- ()
##### Expert Swapping & Offloading
- ()
- ()
- ()

#### Pipeline Scheduling
##### Communication-Computation Co-scheduling
-
-
-
-
-
-
##### Expert Resource Elastic Management
-
-
-
-

#### Hardware Adaptation & Co-design
##### Heterogeneous Compute Resource Coordination
-
-
-
-
##### Domain-Specific Hardware Architecture Design
-
-
-
-
-

#### Distributed & Collaborative Deployment
##### Topology-Aware Communication and Routing
-
-
-
-
-
##### Edge-Cloud Collaborative Inference
-
-
-
##### Cost-Driven Elastic Deployment
-
-
-
---

### Architecture Optimization

#### Efficient Attention
##### Sparse Attention
-
-
-
##### Linear / Kernelized Attention
-
-
-
##### Mixture of Attention Experts
-
-

#### Tailored Routers
##### Token-Aware Sparsity
-
-
-
##### Cache-Aware Routing
-
-
-
##### Load Balance Optimization
-
-
-

#### Diverse Experts
##### Internal Expert Architecture
-
-
-
##### Expert Heterogeneity
-
-
-
-
##### Inter-Expert Parameter Sharing
-
-
-
-
---

### Parameter Optimization


#### Multi-Granularity Quantization
##### Expert-Level Granularity
-
-
-
-
##### Intra-Layer Component Granularity
-
-
-
-
##### Channel-Level Granularity
-
-

#### Low-Rank Approximation
##### Structured Low-Rank Training
-
-
-
##### Post-Training Low-Rank Approximation
-
-
##### Adaptive Rank Selection
-
-
-


#### Pruning
##### Structured Pruning
-
-
-
-
-
##### Unstructured Pruning
-
-
-
-
##### Hybrid Pruning
-
-
-

#### Knowledge Distillation
##### MoE-to-Dense Distillation
-
-

##### MoE-to-Small-MoE Distillation
-
-
-
-
-
-
##### Task-Specific Distillation
-
-
-
---

## 🚀 Application Scenarios

[cite_start]LLMs based on the MoE architecture demonstrate significant potential when deployed at the edge across various latency-critical and privacy-sensitive domains[cite: 1766, 1785]:
* [cite_start]**On-Device Intelligent Assistants**: Supporting real-time conversations, content generation, and context-aware interactions locally on smartphones and wearables[cite: 2774, 2784].
* [cite_start]**Autonomous Driving**: Enabling real-time road condition analysis, V2V collision warning, and trajectory prediction while maintaining a strict 20-100 ms latency constraint without sending sensitive raw sensor data to the cloud[cite: 2791, 2794].
* [cite_start]**Intelligent Healthcare**: Assisting clinicians in local diagnostic reasoning and patient monitoring, mitigating the privacy risks of centralized cloud inference for highly sensitive patient medical records[cite: 2879, 2886].
* [cite_start]**Embodied Robotics**: Operating in smart factories and humanoid platforms with strict 10-100 ms end-to-end latency requirements, reducing massive communication bandwidth overheads while interacting with physical environments[cite: 2895, 2898, 2901].

---

## 📃 Citation

```bibtex
@article{mo2025edge,
  title={Edge MoE: A Survey of Optimization Strategies for Mixture-of-Experts LLMs on the Edge},
  author={Mo, Zhenjia and Zhao, Yong and He, Qiang and Zhang, Mingjin and Chen, Yicong and Li, Ruitao and Qiu, Zihao and Wen, Hao and Chen, Shengyuan and Zhang, Qinggang and Ren, Wei and Cao, Jiannong},
  journal={arXiv preprint},
  year={2025}
}
