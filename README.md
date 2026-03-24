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
- (IEEE'25) **EdgeMoE: Empowering Sparse Large Language Models on Mobile Devices** [[paper]](https://doi.ieeecomputersociety.org/10.1109/TMC.2025.3546466)
- (arXiv'24)**Deep Learning and Machine Learning with GPGPU and CUDA: Unlocking the Power of Parallel Computing** [[paper]](https://arxiv.org/abs/2410.05686)
- (IEEE'24) **Accelerating native inference model performance in edge devices using tensorrt**  [[paper]](https://ieeexplore.ieee.org/document/10690032)
- (ACM'25)** Ktransformers: Unleashing the full potential of cpu/gpu hybrid inference for moe models**[[paper]](https://dl.acm.org/doi/10.1145/3731569.3764843)

##### Expert Caching & Prefetching
- (IEEE'25) **EdgeMoE: Empowering Sparse Large Language Models on Mobile Devices** [[paper]](https://doi.ieeecomputersociety.org/10.1109/TMC.2025.3546466)
- (arXiv'24)**Expertflow: Optimized expert activation and token allocation for efficient mixture-of-experts inference**[[paper]](https://arxiv.org/abs/2410.17954)
- (arXiv'25)**Mixture of cacheconditional experts for efficient mobile device inference**[[paper]](https://arxiv.org/abs/2412.00099)
- (ACL'23)**Adaptive gating in mixture-of-experts based language models**[[paper]](https://aclanthology.org/2023.emnlp-main.217/)

##### Expert Swapping & Offloading
- (ACM'25)**Cache management for mixture-of-experts llms,” in European Conference on Parallel Processing**[[paper]](https://dl.acm.org/doi/10.1007/978-3-031-99872-0_2)
- (IEEE'25)**Serving moe models on resource-constrained edge devices via dynamic expert swapping**[[paper]](https://ieeexplore.ieee.org/document/11022729)
- (IEEE'25)**Ssd offloading for llm mixtureof-experts weights considered harmful in energy efficiency**[[paper]](https://ieeexplore.ieee.org/document/11095626)

#### Pipeline Scheduling
##### Communication-Computation Co-scheduling
- (IEEE'23)**Pipemoe: Accelerating mixture-ofexperts through adaptive pipelining**[[paper]](https://ieeexplore.ieee.org/document/10228874)
- (IEEE'24)**Parm: Efficient training of large sparsely-activated models with dedicated schedules**[[paper]](https://ieeexplore.ieee.org/document/10621327)
- (IEEE'25)**Mast: Efficient training of mixture-of-experts transformers with task pipelining and ordering**[[paper]](https://ieeexplore.ieee.org/document/11183775)
- (NeurIPS'25)**Flowmoe: A scalable pipeline scheduling framework for distributed mixture-of-experts training**[[paper]](https://neurips.cc/virtual/2025/loc/san-diego/poster/118234)
- (IEEE'25)**Mitigating contention in stream multiprocessors for pipelined mixture of experts: An sm-aware scheduling approach**[[paper]](https://ieeexplore.ieee.org/document/11183819)
- (ACM'25)**Harnessing intergpu shared memory for seamless moe communication-computation fusion**[[paper]](https://dl.acm.org/doi/10.1145/3710848.3710868)

##### Expert Resource Elastic Management
- (ACM‘23)**Flexmoe: Scaling large-scale sparse pre-trained model training via dynamic device placement**[[paper]]( https://doi.org/10.1145/3588964)
- (ACM‘25)**Klotski: Efficient mixture-of-expert inference via expertaware multi-batch pipeline**[[paper]](https://dl.acm.org/doi/abs/10.1145/3676641.3716261)
- (ACM‘25)**Harnessing intergpu shared memory for seamless moe communication-computation fusion**[[paper]](https://dl.acm.org/doi/10.1145/3710848.3710868)
- (IEEE'24)**Mpmoe: Memory efficient moe for pre-trained models with adaptive pipeline parallelism**[[paper]](https://ieeexplore.ieee.org/document/10494556)


#### Hardware Adaptation & Co-design
##### Heterogeneous Compute Resource Coordination
- (ICLR'25)**Fiddler: Cpugpu orchestration for fast inference of mixture-of-experts models**[[paper]](https://iclr.cc/virtual/2024/21913)
- (aXiv'25)**eiq neutron: Redefining edge-ai inferencewith integrated npu and compiler innovations**[[paper]]( https://arxiv.org/abs/2509.14388)
- (ACM'25)**Pimoe:Towards efficient moe transformer deployment on npu-pim system
through throttle-aware task offloading**[[paper]](https://dl.acm.org/doi/10.1109/DAC63849.2025.11132528)
- (ACM'24)**Ianus: Integrated accelerator based on npu-pim unified memory system**[[paper]]( https://doi.org/10.1145/3620666.3651324)

##### Domain-Specific Hardware Architecture Design
- (IEEE'21)**Elsa: hardware-software co-design for efficient, lightweight self-attention mechanism in neural networks**[[paper]](https://ieeexplore.ieee.org/document/9499860/)
- (IEEE'22)**Transpim: A memorybased acceleration via software-hardware co-design for transformer**[[paper]](https://ieeexplore.ieee.org/document/9773212)
- (ACM'25)**Slim:A heterogeneous accelerator for edge inference of sparse large
language model via adaptive thresholding**[[paper]](https://doi.org/10.1145/3750727)
- (IEEE'25)**Atleus: Accelerating transformers on the edge enabled by 3d heterogeneous manycore architectures**[[paper]](https://ieeexplore.ieee.org/document/10844861)
- (ICLR'21)**Gshard: Scaling giant models with conditional computation and automatic sharding**[[paper]](https://openreview.net/forum?id=qrwe7XHTmYb)


#### Distributed & Collaborative Deployment
##### Topology-Aware Communication and Routing
- (IJCAI'24)**Locmoe: a low-overhead moe for large language model training**[[paper]](https://doi.org/10.24963/ijcai.2024/705)
- (aXiv'25)**Gracemoe: Grouping and replication with locality-aware routing for efficient distributed moe inference**[[paper]](https://arxiv.org/abs/2509.25041)
- (IEEE'24)**Exploiting inter-layer expert affinity for accelerating mixture-of-experts model inference**[[paper]](https://ieeexplore.ieee.org/document/10579139)
- (ACM'24)**“Schemoe: An extensible mixture-of-experts distributed training system with tasks scheduling**[[paper]](https://doi.org/10.1145/3627703.3650083)
- (USENIX ATC'23)**Accelerating distributed {MoE} training and inference with lina**[[paper]](https://www.usenix.org/conference/atc23/presentation/li-jiamin)
##### Edge-Cloud Collaborative Inference
- (aXiv'25)**Ec2moe: Adaptive end-cloud pipeline collaboration enabling scalable mixture-of-experts inference**[[paper]](https://arxiv.org/abs/2508.06024)
- (IEEE'25)**Multi-tier multi-node scheduling of llm for collaborative ai computing**[[paper]](https://ieeexplore.ieee.org/document/11044698)
- (IEEE'24)**Exploiting inter-layer expert affinity for accelerating mixture-of-experts model inference**[[paper]](https://ieeexplore.ieee.org/document/10579139)

##### Cost-Driven Elastic Deployment
- (IEEE'24)**Moesys: A distributed and efficient mixture-of-experts training and inference system for internet services**[[paper]](https://ieeexplore.ieee.org/document/10528887)
- (USENIX ATC'23)**Accelerating distributed {MoE} training and inference with lina**[[paper]](https://www.usenix.org/conference/atc23/presentation/li-jiamin)
##### Edge-Cloud Collaborative Inference
- (IEEE'25)**“Optimizing distributed deployment of mixture-of-experts model inference in serverless computing**[[paper]](https://ieeexplore.ieee.org/document/11044553)
---

### Architecture Optimization

#### Efficient Attention
##### Sparse Attention
- (IEEE'21)**Spatten: Efficient sparse attention architecture with cascade token and head pruning**[[paper]](https://ieeexplore.ieee.org/document/9407232)
- (ICML'24)**Quest:query-aware sparsity for efficient long-context llm inference**[[paper]](https://dl.acm.org/doi/10.5555/3692070.3694025)
- (NeurIPS'24)**Infllm: Training-free long-context extrapolation for llms with an efficient context memory**[[paper]](https://proceedings.neurips.cc/paper_files/paper/2024/file/d842425e4bf79ba039352da0f658a906-Paper-Conference.pdf)

##### Linear / Kernelized Attention
- (ICLR'25)**LoLCATs: On low-rank linearizing of large language models**[[paper]](https://openreview.net/forum?id=8VtGeyJyx9)
- (ACM'25)**Elfatt: Efficient linear fast attention for vision transformers**[[paper]](https://doi.org/10.1145/3746027.3754825)
- (PMLR'24)**Mobile attention: Mobile-friendly linear-attention for vision transformers**[[paper]](https://proceedings.mlr.press/v235/yao24c.html)

##### Mixture of Attention Experts
- (EMNLP'22)**Mixture of attention heads: Selecting attention heads per token**[[paper]](https://www.semanticscholar.org/paper/3820231d31540ecb05d94c74d959a2f61d3136ea)
- (NeurIPS'24)**Switchhead:Accelerating transformers with mixture-of-experts attention**[[paper]](https://proceedings.neurips.cc/paper_files/paper/2024/file/87be61bf9338389702712f5e9754a986-Paper-Conference.pdf)


#### Tailored Routers
##### Token-Aware Sparsity
- (ACL'24)**Harder task needs more experts: Dynamic routing in MoE models**[[paper]](https://aclanthology.org/2024.acl-long.696/)
- (ACL'23)**Adaptive gating in mixture-of-experts based language models**[[paper]](https://aclanthology.org/2023.emnlp-main.217/)
- (ACM'25)**AdapMoE: Adaptive Sensitivity-based Expert Gating and Management for Efficient MoE Inference**[[paper]](https://doi.org/10.1145/3676536.3676741)
##### Cache-Aware Routing
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()
##### Load Balance Optimization
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()

#### Diverse Experts
##### Internal Expert Architecture
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()
##### Expert Heterogeneity
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()

##### Inter-Expert Parameter Sharing
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()
---

### Parameter Optimization


#### Multi-Granularity Quantization
##### Expert-Level Granularity
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()
##### Intra-Layer Component Granularity
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()
##### Channel-Level Granularity
- ()** **[[paper]]()
- ()** **[[paper]]()


#### Low-Rank Approximation
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()

##### Post-Training Low-Rank Approximation
- ()** **[[paper]]()
- ()** **[[paper]]()

##### Adaptive Rank Selection
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()


#### Pruning
##### Structured Pruning
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()

##### Unstructured Pruning
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()
##### Hybrid Pruning
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()

#### Knowledge Distillation
##### MoE-to-Dense Distillation
- ()** **[[paper]]()
- ()** **[[paper]]()



##### MoE-to-Small-MoE Distillation
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()

##### Task-Specific Distillation
- ()** **[[paper]]()
- ()** **[[paper]]()
- ()** **[[paper]]()

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
