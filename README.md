# Awesome Edge MoE: Optimization Strategies for LLMs on the Edge

<div align="center">
     <a href="#" target="_blank"><img src="https://img.shields.io/badge/Paper-Arxiv-red?logo=arxiv&style=flat-square" alt="arXiv"></a>
     <a href="https://github.com/ZajacMo/When-MoE-Meets-Edge"><img src="https://img.shields.io/github/stars/ZajacMo/When-MoE-Meets-Edge"/></a>
     <a href="https://github.com/ZajacMo/When-MoE-Meets-Edge"><img src="https://img.shields.io/github/forks/ZajacMo/When-MoE-Meets-Edge"/></a>
</div>

[cite_start]This repository provides a comprehensive collection of research papers, open-source projects, and optimization strategies for deploying **Mixture-of-Experts (MoE) Large Language Models on Edge Devices**[cite: 1743]. [cite_start]It includes contents from our survey paper 📖<em>"**Edge MoE: A Survey of Optimization Strategies for Mixture-of-Experts LLMs on the Edge**"</em> and will be continuously updated[cite: 1739, 1750].

🤗 **You are very welcome to contribute to this repository** by launching an issue or a pull request. 

[cite_start]📫 **Contact us via emails:** `zhaoyong@uestc.edu.cn` [cite: 1752]

---

<div>
<h3 align="center">
       <p align="center"><img width="100%" src="figures/illustration_edge_moe_overview.png" alt="Overview of optimization strategies for Edge MoE"/></p>
    <p align="center"><em>Overview of optimization strategies for MoE-based LLMs on edge devices, covering system, architecture, and parameter levels.</em></p>
</div>

## 📜 Catalog

> **[Awesome Edge MoE](#awesome-edge-moe)**
>
> - **[🔥 News](#-news)**
> - **[📖 Overview](#-overview)**
> - **[🪴 Taxonomy](#-taxonomy)**
>   - [System Optimization](#system-optimization)
>   - [Architecture Optimization](#architecture-optimization)
>   - [Parameter Optimization](#parameter-optimization)
> - **[🚀 Application Scenarios](#-application-scenarios)**
> - **[📃 Citation](#-citation)**

---

## 🔥 News

* [cite_start]**[2026-03]** 🔥🔥 Our survey on Edge MoE optimization strategies is released, alongside this repository! [cite: 1750]

## 🪴 Taxonomy

### System Optimization

<p align="center"><img width="100%" src="figures/system_optimization.png" alt="System Optimization Taxonomy" /></p>

#### Memory Management
* [cite_start]**Hierarchical Storage**: EdgeMoE, Li et al., TensorRT-LLM, KTransformers [cite: 1869]
* [cite_start]**Expert Caching & Prefetching**: EdgeMoE, ExpertFlow, Skliar et al., Li et al. [cite: 1870]
* [cite_start]**Expert Swapping & Offloading**: Angelopoulos et al., PC-MoE, Kyung et al. [cite: 1871]

#### Pipeline Scheduling
* [cite_start]**Communication-Computation Co-scheduling**: PipeMoE, Parm, Mast, FlowMoE, Pan et al., CCFuser [cite: 1872]
* [cite_start]**Expert Resource Elastic Management**: FlexMoE, KLOTSKI, CCFuser, MPMOE [cite: 1873]

#### Hardware Adaptation & Co-design
* [cite_start]**Heterogeneous Compute Resource Coordination**: Fiddler, eIQ Neutron, PIMOE, IANUS [cite: 1881]
* [cite_start]**Domain-Specific Hardware Architecture Design**: ELSA, TransPIM, SLIM, Atleus, GShard [cite: 1881, 1882]

#### Distributed & Collaborative Deployment
* [cite_start]**Topology-Aware Communication and Routing**: LocMoE, GRACE-MoE, ExFlow, ScheMoE, Lina [cite: 1882]
* [cite_start]**Edge-Cloud Collaborative Inference**: EC2MoE, MMSL, ExFlow [cite: 1883]
* [cite_start]**Cost-Driven Elastic Deployment**: MoESys, Lina, Liu et al. [cite: 1884]

---

### Architecture Optimization

<p align="center"><img width="100%" src="figures/architecture_optimization.png" alt="Architecture Optimization Taxonomy" /></p>

#### Efficient Attention
* [cite_start]**Sparse Attention**: SpAtten, Quest, InfLLM [cite: 1885]
* [cite_start]**Linear / Kernelized Attention**: LoLCATs, ELFATT, Mobile Attention [cite: 1886]
* [cite_start]**Mixture of Attention Experts**: MoA, SwitchHead [cite: 1890]

#### Tailored Routers
* [cite_start]**Token-Aware Sparsity**: Harder Task, Li et al., AdapMoE [cite: 1892]
* [cite_start]**Cache-Aware Routing**: Skliar et al., ExpertFlow, ProMoE [cite: 1898]
* [cite_start]**Load Balance Optimization**: Huang et al., CCFuser, ReMoE [cite: 1901]

#### Diverse Experts
* [cite_start]**Internal Expert Architecture**: LiteMoE, SwapMoE, HMOE [cite: 1903]
* [cite_start]**Expert Heterogeneity**: EdgeMoE, CoEL, D²MoE, HOBBIT [cite: 1927]
* [cite_start]**Inter-Expert Parameter Sharing**: DeepSeekMoE, D²-MoE, MoE-SVD, GenPoE [cite: 1928]

---

### Parameter Optimization

<p align="center"><img width="100%" src="figures/parameter_optimization.png" alt="Parameter Optimization Taxonomy" /></p>

#### Multi-Granularity Quantization
* [cite_start]**Expert-Level Granularity**: MoPEQ, GEMQ, PC-MoE, AdapMoE [cite: 1929]
* [cite_start]**Intra-Layer Component Granularity**: MxMoE, Edge-MPQ, PIMOE, Block-Wise [cite: 1930]
* [cite_start]**Channel-Level Granularity**: Automated Fine-Grained, Oiso [cite: 1931]

#### Low-Rank Approximation
* [cite_start]**Structured Low-Rank Training**: Ultra-Memory-Efficient, QLORA, Choi [cite: 1932]
* [cite_start]**Post-Training Low-Rank Approximation**: QMoE, Mixture Compressor [cite: 1933]
* [cite_start]**Adaptive Rank Selection**: MoRE, LoRAMOE, Cannikin [cite: 1934]

#### Pruning
* [cite_start]**Structured Pruning**: Switch Transformers, PC-MoE, Pre-gated MoE, CALM, Memory³ [cite: 1935]
* [cite_start]**Unstructured Pruning**: TransCODE, Mobile Transformer, EfficientMoE, MegaBlocks [cite: 1936]
* [cite_start]**Hybrid Pruning**: Mixture Compressor, Expert Choice, MPMOE [cite: 1937]

#### Knowledge Distillation
* [cite_start]**MoE-to-Dense Distillation**: Switch Transformers, One Student [cite: 1938]
* [cite_start]**MoE-to-Small-MoE Distillation**: SlimMoE, Scaling VLM, LLaVA-MoD, MoDE, D2DMoE, DeepMoE [cite: 1939]
* [cite_start]**Task-Specific Distillation**: SubDistill, Muppet, EdgeMoE [cite: 1940]

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
