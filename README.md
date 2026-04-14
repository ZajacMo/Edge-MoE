
# Awesome Edge MoE: A Survey of Optimization Strategies for Mixture-of-Experts LLMs on the Edge

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

- (arXiv'25) **A Comprehensive Survey of Mixture-of-Experts: Algorithms, Theory, and Applications** [[paper]](https://arxiv.org/abs/2503.07137)
- (arXiv'24) **A Survey on Mixture of Experts in Large Language Models**[[paper]](https://arxiv.org/abs/2407.06204)
- (ACM CSUR'24) **A Review on Edge Large Language Models: Design, Execution, and Applications**[[paper]](https://dl.acm.org/doi/full/10.1145/3719664)
- (TMLR'24) **Efficient Large Language Models: A Survey**[[paper]](https://arxiv.org/abs/2312.03863)
- (INLG'2025) **Taming the Titans: A Survey of Efficient LLM Inference Serving**[[paper]](https://aclanthology.org/2025.inlg-main.32/)
- (Proc. IEEE'24) **Edge intelligence: Paving the last mile of artificial intelligence with edge computing**[[paper]](https://ieeexplore.ieee.org/document/8736011)
- (COMST'17) **Mobile edge computing: A survey on architecture and computation offloading**[[paper]](https://ieeexplore.ieee.org/document/7879258)
- (COMST'17) **A survey on mobile edge computing: The communication perspective**[[paper]](https://ieeexplore.ieee.org/document/8016573)
- (Computer'17) **The emergence of edge computing**[[paper]](https://ieeexplore.ieee.org/document/7807196)
- (IoT-J'16) **Edge computing: Vision and challenges**[[paper]](https://ieeexplore.ieee.org/document/7488250)
- (COMST'29) **Convergence of edge computing and deep learning: A comprehensive survey**[[paper]](https://ieeexplore.ieee.org/document/8976180)
- (arXiv'20) **Communication-Efficient edge ai: Algorithms and systems**[[paper]](https://arxiv.org/abs/2002.09668)
- (COMST'20) **Federated learning in mobile edge networks: A comprehensive survey**[[paper]](https://ieeexplore.ieee.org/document/9060868)
- (COMST'21) **Federated learning for internet of things: A comprehensive survey**[[paper]](https://ieeexplore.ieee.org/document/9415623)
- (COMST'21) **Federated learning for internet of things: Recent advances, taxonomy, and open challenges**[[paper]](https://ieeexplore.ieee.org/document/9460016)
- (COMST'25) **Mobile edge intelligence for large language models: A contemporary survey**[[paper]](https://ieeexplore.ieee.org/document/10835069)
- (TKDE'25) **A survey on mixture of experts in large language models**[[paper]](https://ieeexplore.ieee.org/document/10937907)


## 🪴 Taxonomy

### System Optimization
#### Memory Management
##### Hierarchical Storage
- (TMC'25) **EdgeMoE: Empowering Sparse Large Language Models on Mobile Devices** [[paper]](https://doi.ieeecomputersociety.org/10.1109/TMC.2025.3546466)
- (arXiv'24) **Deep Learning and Machine Learning with GPGPU and CUDA: Unlocking the Power of Parallel Computing** [[paper]](https://arxiv.org/abs/2410.05686)
- (RAICS'24) **Accelerating native inference model performance in edge devices using tensorrt**  [[paper]](https://ieeexplore.ieee.org/document/10690032)
- (SOSP'25) **Ktransformers: Unleashing the full potential of cpu/gpu hybrid inference for moe models**[[paper]](https://dl.acm.org/doi/10.1145/3731569.3764843)

##### Expert Caching & Prefetching
- (TMC'25) **EdgeMoE: Empowering Sparse Large Language Models on Mobile Devices** [[paper]](https://doi.ieeecomputersociety.org/10.1109/TMC.2025.3546466)
- (arXiv'24) **Expertflow: Optimized expert activation and token allocation for efficient mixture-of-experts inference**[[paper]](https://arxiv.org/abs/2410.17954)
- (arXiv'25) **Mixture of cache-conditional experts for efficient mobile device inference**[[paper]](https://arxiv.org/abs/2412.00099)
- (ACL'23) **Adaptive gating in mixture-of-experts based language models**[[paper]](https://aclanthology.org/2023.emnlp-main.217/)

##### Expert Swapping & Offloading
- (Euro-Par'25) **Cache management for mixture-of-experts llms,” in European Conference on Parallel Processing**[[paper]](https://dl.acm.org/doi/10.1007/978-3-031-99872-0_2)
- (TC'25'25) **Serving moe models on resource-constrained edge devices via dynamic expert swapping**[[paper]](https://ieeexplore.ieee.org/document/11022729)
- (CAL'25) **Ssd offloading for llm mixture-of-experts weights considered harmful in energy efficiency**[[paper]](https://ieeexplore.ieee.org/document/11095626)

#### Pipeline Scheduling
##### Communication-Computation Co-scheduling
- (INFOCOM'23) **Pipemoe: Accelerating mixture-of-experts through adaptive pipelining**[[paper]](https://ieeexplore.ieee.org/document/10228874)
- (INFOCOM'24) **Parm: Efficient training of large sparsely-activated models with dedicated schedules**[[paper]](https://ieeexplore.ieee.org/document/10621327)
- (ICDCS'25) **Mast: Efficient training of mixture-of-experts transformers with task pipelining and ordering**[[paper]](https://ieeexplore.ieee.org/document/11183775)
- (NeurIPS'25) **Flowmoe: A scalable pipeline scheduling framework for distributed mixture-of-experts training**[[paper]](https://neurips.cc/virtual/2025/loc/san-diego/poster/118234)
- (ICDCS'25) **Mitigating contention in stream multiprocessors for pipelined mixture of experts: An sm-aware scheduling approach**[[paper]](https://ieeexplore.ieee.org/document/11183819)
- (PPOPP'25) **Harnessing inter-GPU shared memory for seamless moe communication-computation fusion**[[paper]](https://dl.acm.org/doi/10.1145/3710848.3710868)

##### Expert Resource Elastic Management
- (PACMMOD'23) **Flexmoe: Scaling large-scale sparse pre-trained model training via dynamic device placement**[[paper]]( https://doi.org/10.1145/3588964)
- (ASPLO'25) **Klotski: Efficient mixture-of-expert inference via expert-aware multi-batch pipeline**[[paper]](https://dl.acm.org/doi/abs/10.1145/3676641.3716261)
- (PPOPP'25) **Harnessing inter-GPU shared memory for seamless moe communication-computation fusion**[[paper]](https://dl.acm.org/doi/10.1145/3710848.3710868)
- (TPDS'24) **Mpmoe: Memory efficient moe for pre-trained models with adaptive pipeline parallelism**[[paper]](https://ieeexplore.ieee.org/document/10494556)


#### Hardware Adaptation & Co-design
##### Heterogeneous Compute Resource Coordination
- (ICLR'25) **Fiddler: Cpu-GPU orchestration for fast inference of mixture-of-experts models**[[paper]](https://iclr.cc/virtual/2024/21913)
- (aXiv'25) **eiq neutron: Redefining edge-ai inferencewith integrated npu and compiler innovations**[[paper]]( https://arxiv.org/abs/2509.14388)
- (DAC'25) **Pimoe:Towards efficient moe transformer deployment on npu-pim system
through throttle-aware task offloading**[[paper]](https://dl.acm.org/doi/10.1109/DAC63849.2025.11132528)
- (ASPLOS'24) **Ianus: Integrated accelerator based on npu-pim unified memory system**[[paper]]( https://doi.org/10.1145/3620666.3651324)

##### Domain-Specific Hardware Architecture Design
- (ISCA'21) **Elsa: hardware-software co-design for efficient, lightweight self-attention mechanism in neural networks**[[paper]](https://ieeexplore.ieee.org/document/9499860/)
- (HPCA'22) **Transpim: A memory-based acceleration via software-hardware co-design for transformer**[[paper]](https://ieeexplore.ieee.org/document/9773212)
- (TECS'25) **Slim:A heterogeneous accelerator for edge inference of sparse large language model via adaptive thresholding**[[paper]](https://doi.org/10.1145/3750727)
- (TCAD'25) **Atleus: Accelerating transformers on the edge enabled by 3d heterogeneous manycore architectures**[[paper]](https://ieeexplore.ieee.org/document/10844861)
- (ICLR'21) **Gshard: Scaling giant models with conditional computation and automatic sharding**[[paper]](https://openreview.net/forum?id=qrwe7XHTmYb)


#### Distributed & Collaborative Deployment
##### Topology-Aware Communication and Routing
- (IJCAI'24) **Locmoe: a low-overhead moe for large language model training**[[paper]](https://doi.org/10.24963/ijcai.2024/705)
- (aXiv'25) **Grace-moe: Grouping and replication with locality-aware routing for efficient distributed moe inference**[[paper]](https://arxiv.org/abs/2509.25041)
- (IPDPS'24) **Exploiting inter-layer expert affinity for accelerating mixture-of-experts model inference**[[paper]](https://ieeexplore.ieee.org/document/10579139)
- (EuroSys'24) **“Schemoe: An extensible mixture-of-experts distributed training system with tasks scheduling**[[paper]](https://doi.org/10.1145/3627703.3650083)
- (USENIX ATC'23) **Accelerating distributed {MoE} training and inference with lina**[[paper]](https://www.usenix.org/conference/atc23/presentation/li-jiamin)

##### Edge-Cloud Collaborative Inference
- (aXiv'25) **Ec2moe: Adaptive end-cloud pipeline collaboration enabling scalable mixture-of-experts inference**[[paper]](https://arxiv.org/abs/2508.06024)
- (INFOCOM'25) **Multi-tier multi-node scheduling of llm for collaborative ai computing**[[paper]](https://ieeexplore.ieee.org/document/11044698)
- (IPDPS'24) **Exploiting inter-layer expert affinity for accelerating mixture-of-experts model inference**[[paper]](https://ieeexplore.ieee.org/document/10579139)

##### Cost-Driven Elastic Deployment
- (TSC'24) **Moesys: A distributed and efficient mixture-of-experts training and inference system for internet services**[[paper]](https://ieeexplore.ieee.org/document/10528887)
- (USENIX ATC'23) **Accelerating distributed {MoE} training and inference with lina**[[paper]](https://www.usenix.org/conference/atc23/presentation/li-jiamin)
- (INFOCOM'25) **“Optimizing distributed deployment of mixture-of-experts model inference in serverless computing**[[paper]](https://ieeexplore.ieee.org/document/11044553)
---

### Architecture Optimization

#### Efficient Attention
##### Sparse Attention
- (HPCA'21) **Spatten: Efficient sparse attention architecture with cascade token and head pruning**[[paper]](https://ieeexplore.ieee.org/document/9407232)
- (ICML'24) **Quest:query-aware sparsity for efficient long-context llm inference**[[paper]](https://dl.acm.org/doi/10.5555/3692070.3694025)
- (NeurIPS'24) **Infllm: Training-free long-context extrapolation for llms with an efficient context memory**[[paper]](https://proceedings.neurips.cc/paper_files/paper/2024/file/d842425e4bf79ba039352da0f658a906-Paper-Conference.pdf)

##### Linear / Kernelized Attention
- (ICLR'25) **LoLCATs: On low-rank linearizing of large language models**[[paper]](https://openreview.net/forum?id=8VtGeyJyx9)
- (MM'25) **Elfatt: Efficient linear fast attention for vision transformers**[[paper]](https://doi.org/10.1145/3746027.3754825)
- (PMLR'24) **Mobile attention: Mobile-friendly linear-attention for vision transformers**[[paper]](https://proceedings.mlr.press/v235/yao24c.html)

##### Mixture of Attention Experts
- (EMNLP'22) **Mixture of attention heads: Selecting attention heads per token**[[paper]](https://www.semanticscholar.org/paper/3820231d31540ecb05d94c74d959a2f61d3136ea)
- (NeurIPS'24) **Switchhead:Accelerating transformers with mixture-of-experts attention**[[paper]](https://proceedings.neurips.cc/paper_files/paper/2024/file/87be61bf9338389702712f5e9754a986-Paper-Conference.pdf)


#### Tailored Routers
##### Token-Aware Sparsity
- (ACL'24) **Harder task needs more experts: Dynamic routing in MoE models**[[paper]](https://aclanthology.org/2024.acl-long.696/)
- (ACL'23) **Adaptive gating in mixture-of-experts based language models**[[paper]](https://aclanthology.org/2023.emnlp-main.217/)
- (ICCAD'25) **AdapMoE: Adaptive Sensitivity-based Expert Gating and Management for Efficient MoE Inference**[[paper]](https://doi.org/10.1145/3676536.3676741)

##### Cache-Aware Routing
- (TMLR'25) **Mixture of cache-conditional experts for efficient mobile device inference**[[paper]](https://arxiv.org/abs/2412.00099)
- (arXiv'24) **Expertflow: Optimized expert activation and token allocation for efficient mixture-of-experts inference**[[paper]](https://arxiv.org/abs/2410.17954)
- (arXiv'24) **Promoe: Fast moe-based llm serving using proactive caching**[[paper]](https://arxiv.org/abs/2410.22134)

##### Load Balance Optimization
- (NeurIPS'24) **Toward efficient inference for mixture of experts**[[paper]](https://proceedings.neurips.cc/paper_files/paper/2024/hash/98bf3b8505c611ac21055dd9d355c66e-Abstract-Conference.html)
- (PPOPP'25) **Harnessing inter-GPU shared memory for seamless moe communication-computation fusion**[[paper]](https://dl.acm.org/doi/10.1145/3710848.3710868)
- (ICLR'25) **Remoe: Fully differentiable mixture-of-experts with reLU routing**[[paper]](https://openreview.net/forum?id=4D0f16Vwc3)

#### Diverse Experts
##### Internal Expert Architecture
- (SenSys'24) **Litemoe: Customizing on-device llm serving via proxy submodel tuning**[[paper]](https://doi.org/10.1145/3666025.3699355)
- (ACL'24) **Swapmoe: Serving off-the-shelf moe-based large language models with tunable memory budget**[[paper]](https://aclanthology.org/2024.acl-long.363/)
- (EMNLP'25) **HMoE: Heterogeneous mixture of experts for language modeling**[[paper]](https://aclanthology.org/2025.emnlp-main.1115/)

##### Expert Heterogeneity
- (TMC'25) **EdgeMoE: Empowering Sparse Large Language Models on Mobile Devices** [[paper]](https://doi.ieeecomputersociety.org/10.1109/TMC.2025.3546466)
- (COMMAG'25) **The moe-empowered edge llms deployment: Architecture, challenges, and opportunities**[[paper]](https://ieeexplore.ieee.org/document/11141664)
- (MobiCom'25) **D2MoE: Dual Routing and Dynamic Scheduling for Efficient On-Device MoE-based LLM Serving**[[paper]](https://dl.acm.org/doi/10.1145/3680207.3723493)
- (aXiv'24) **Hobbit: A mixed precision expert offloading system for fast moe inference**[[paper]](https://doi.org/10.48550/arXiv.2411.01433)

##### Inter-Expert Parameter Sharing
- (ACL'24) **DeepSeekMoE: Towards ultimate expert specialization in mixture-of-experts language models**[[paper]](https://aclanthology.org/2024.acl-long.70/)
- (ICML'25) **Delta decompression for moe-based LLMs compression**[[paper]](https://openreview.net/forum?id=ziezViPoN1)
- (ICML'25) **Moe-SVD: Structured mixture-of-experts LLMs compression via singular value decomposition**[[paper]](https://openreview.net/forum?id=acJ3vdFljk)
- (EMNLP'25) **Genpoe: Generative passage-level mixture of experts for knowledge enhancement of llms**[[paper]](https://aclanthology.org/2025.findings-emnlp.272/)
---

### Parameter Optimization


#### Multi-Granularity Quantization
##### Expert-Level Granularity
- (ICCV'25) **Mopeq: Mixture of mixed precision quantized experts**[[paper]](https://ieeexplore.ieee.org/document/11376553)
- (ICLR'26) **Towards global expert-level mixed-precision quantization for mixture-of-experts LLMs**[[paper]](https://openreview.net/forum?id=wAc718O8UM)
-  (TC'25) **Serving moe models on resource-constrained edge devices via dynamic expert swapping**[[paper]](https://ieeexplore.ieee.org/document/11022729)
- (ICCAD'25) **AdapMoE: Adaptive Sensitivity-based Expert Gating and Management for Efficient MoE Inference**[[paper]](https://doi.org/10.1145/3676536.3676741)

##### Intra-Layer Component Granularity
- (ICML'25) **Mxmoe: Mixed-precision quantization for moe with accuracy and performance co-design**[[paper]](:https://openreview.net/forum?id=pXoZLGMNDm)
- (TC'24) **Edgempq: Layer-wise mixed-precision quantization with tightly integrated versatile inference units for edge computing**[[paper]](https://www.computer.org/csdl/journal/tc/2024/11/10633877/1ZlBglVrtZK)
- (DAC'25) **Pimoe:Towards efficient moe transformer deployment on npu-pim system through throttle-aware task offloading**[[paper]](https://dl.acm.org/doi/10.1109/DAC63849.2025.11132528)
- (TCAD'24) **Block-wise mixed-precision quantization: Enabling high efficiency for practical reram-based dnn accelerators**[[paper]](https://ieeexplore.ieee.org/document/10547183)

##### Channel-Level Granularity
- (ACL'25) **Automated fine-grained mixture-of-experts quantization**[[paper]](https://aclanthology.org/2025.findings-acl.1386/)
- (TCAD'25) **Oiso:Outlier-isolated data format for low-bit large language model quantization**[[paper]](https://ieeexplore.ieee.org/document/11062568)

#### Low-Rank Approximation
##### Structured Low-Rank Approximation
- (TCAD'25) **Ultra memory-efficient on-fpga training of transformers via tensor-compressed optimization**[[paper]](https://ieeexplore.ieee.org/document/11121368)
- (NeurIPS'23) **Qlora:efficient finetuning of quantized llms**[[paper]](https://proceedings.neurips.cc/paper_files/paper/2023/file/1feb87871436031bdc0f2beaa62a049b-Paper-Conference.pdf)
- (Access'25) **Toward generating quality test questions and answers using quantized low-rank adapters in llms**[[paper]](https://ieeexplore.ieee.org/document/11005578)

##### Post-Training Low-Rank Approximation
- (aXiv'23) **Qmoe: Practical sub-1-bit compression of trillion-parameter models**[[paper]](https://arxiv.org/abs/2310.16795)
- (ICLR'25) **Mixture compressor for mixture-of-experts LLMs gains more**[[paper]](https://openreview.net/forum?id=hheFYjOsWO)

##### Adaptive Rank Selection
- (ACL'25) **MoRE: A mixture of low-rank experts for adaptive multi-task learning**[[paper]](https://aclanthology.org/2025.findings-acl.68/)
- (ACL'24) **LoRAMoE: Alleviating world knowledge forgetting in large language models via MoE-style plugin**[[paper]](https://aclanthology.org/2024.acl-long.106/)
- (TPDS'25) **Cannikin:No lagger of slo in concurrent multiple lora llm serving**[[paper]](https://ieeexplore.ieee.org/document/11082562)


#### Pruning
##### Structured Pruning
- (JMLR'22) **Switch transformers: scaling to trillion parameter models with simple and efficient sparsity**[[paper]](https://dl.acm.org/doi/10.5555/3586589.3586709)
- (TC'25) **Serving moe models on resource-constrained edge devices via dynamic expert swapping**[[paper]](https://ieeexplore.ieee.org/document/11022729)
- (ISCA'24) **Pre-gated moe: An algorithm-system co-design for fast and scalable mixture-of-expert inference**[[paper]](https://www.computer.org/csdl/proceedings-article/isca/2024/265800b018/1Z3pEe79xPW)
- (NeurIPS'22) **Confident adaptive language modeling**[[paper]](https://papers.neurips.cc/paper_files/paper/2022/file/6fac9e316a4ae75ea244ddcef1982c71-Paper-Conference.pdf)
- (JMLR'24) **Memory3 : Language modeling with explicit memory**[[paper]](http://dx.doi.org/10.4208/jml.240708)

##### Unstructured Pruning
- (TCAD'23) **Transcode: Co-design of transformers and accelerators for efficient training and inference**[[paper]](https://ieeexplore.ieee.org/document/10144614)
- (TCAD'24) **Mobile transformer accelerator exploiting various line sparsity and tile-based dynamic quantization**[[paper]](https://ieeexplore.ieee.org/document/10375766)
- (TPDS'25) **Efficientmoe: Optimizing mixture-of-experts model training with adaptive load balance**[[paper]](https://ieeexplore.ieee.org/document/10876795)
- (aXiv'22) **Megablocks:Efficient sparse training with mixture-of-experts**[[paper]](https://arxiv.org/abs/2211.15841)

##### Hybrid Pruning
- (ICLR'25) **Mixture compressor for mixture-of-experts LLMs gains more**[[paper]](https://openreview.net/forum?id=hheFYjOsWO)
- (NeurIPS'22) **Mixture-of-experts with expert choice routing**[[paper]](https://papers.neurips.cc/paper_files/paper/2022/file/2f00ecd787b432c1d36f3de9800728eb-Paper-Conference.pdf)
- (IPDPS'23) **Mpipemoe: Memory efficient moe for pre-trained models with adaptive pipeline parallelism**[[paper]](https://ieeexplore.ieee.org/document/10177396)

#### Knowledge Distillation
##### MoE-to-Dense Distillation
- (JMLR'22) **Switch transformers: scaling to trillion parameter models with simple and efficient sparsity**[[paper]](https://dl.acm.org/doi/10.5555/3586589.3586709)
- (aXiv'22) **One student knows all experts know: From sparse to dense**[[paper]](https://arxiv.org/abs/2201.10890)

##### MoE-to-Small-MoE Distillation
- (COLM'25) **Slimmoe: Structured compression of large moe models via expert slimming and distillation**[[paper]](https://openreview.net/forum?id=oaCUsn391F)
- (EMNLP'23) **Scaling vision-language models with sparse mixture of experts**[[paper]](https://aclanthology.org/2023.findings-emnlp.758/)
- (ICLR'25) **LLaVA-mod: Making LLaVA tiny via moe-knowledge distillation**[[paper]](https://openreview.net/forum?id=uWtLOy35WD)
- (AAAI'24) **“Mode: a mixture-of-experts model with mutual distillation among the experts**[[paper]](https://ojs.aaai.org/index.php/AAAI/article/view/29539)
- (NeurIPS'24) **Exploiting activation sparsity with dense to dynamic-k mixture-of-experts conversion**[[paper]](https://proceedings.neurips.cc/paper_files/paper/2024/file/4c2092ec0b1370cce3fb5965ab255fae-Paper-Conference.pdf)
- (PMLR'20) **Deep mixture of experts via shallow embedding**[[paper]](https://proceedings.mlr.press/v115/wang20d.html)

##### Task-Specific Distillation
- (aXiv'26) **Distilling lightweight domain experts from large ml models by identifying relevant subspaces**[[paper]](https://arxiv.org/abs/2601.05913)
- (EMNLP'21) **Muppet: Massive multi-task representations with pre-finetuning**[[paper]](https://aclanthology.org/2021.emnlp-main.468/)
- (TMC'25) **EdgeMoE: Empowering Sparse Large Language Models on Mobile Devices** [[paper]](https://doi.ieeecomputersociety.org/10.1109/TMC.2025.3546466)

---

## 🚀 Application Scenarios



### On-Device Intelligent Assistants: 
Supporting real-time conversations, content generation, and context-aware interactions locally on smartphones and wearables
- (TMC'25) **EdgeMoE: Empowering Sparse Large Language Models on Mobile Devices** [[paper]](https://doi.ieeecomputersociety.org/10.1109/TMC.2025.3546466)
- (SAGE'23) **Towards large language models at the edge on mobile, augmented reality, and virtual reality devices with unity** [[paper]](https://openreview.net/forum?id=ahVsd1hy2W)
- (aXiv'25) **A Comprehensive Survey of Mixture-of-Experts: Algorithms, Theory, and Applications** [[paper]](https://arxiv.org/abs/2503.07137)
- (ICML'24) **Mobilellm: Optimizing sub-billion parameter language models for on-device use cases** [[paper]](https://dl.acm.org/doi/10.5555/3692070.3693386)
- (SOSP'24) **Powerinfer: Fast large language model serving with a consumer-grade gpu** [[paper]](https://dl.acm.org/doi/10.1145/3694715.3695964)

### Autonomous Driving: 
Enabling real-time road condition analysis, V2V collision warning, and trajectory prediction while maintaining a strict 20-100 ms latency constraint without sending sensitive raw sensor data to the cloud.
- (COMST'25) **Mobile edge intelligence for large language models: A contemporary survey**[[paper]](https://ieeexplore.ieee.org/document/10835069)
- (aXiv'17) **Outrageously large neural networks: The sparsely-gated mixture-of-experts layer** [[paper]](https://arxiv.org/abs/1701.06538)
- (JMLR'22) **Switch transformers: scaling to trillion parameter models with simple and efficient sparsity**[[paper]](https://dl.acm.org/doi/10.5555/3586589.3586709)
- (Computer'17) **The emergence of edge computing**[[paper]](https://ieeexplore.ieee.org/document/7807196)
- (IoT-J'16) **Edge computing: Vision and challenges**[[paper]](https://ieeexplore.ieee.org/document/7488250)
- (AAAI'25) **Language prompt for autonomous driving** [[paper]](https://dl.acm.org/doi/10.1609/aaai.v39i8.32902)
- (aXiv'23) ** Can you text what is happening? Integrating pre-trained language encoders into trajectory prediction models for autonomous driving** [[paper]](https://arxiv.org/abs/2309.05282)
- (aXiv'23) **Gpt-driver: Learning to drive with gpt** [[paper]](https://arxiv.org/abs/2310.01415)
- (WACV'24) **Drive as you speak: Enabling human-like interaction with large language models in autonomous vehicles** [[paper]]()
- (CVPR'23) **Planning-oriented autonomous driving** [[paper]](https://ieeexplore.ieee.org/document/10205112)
- (TMC'24) **Pacp: Priority-aware collaborative perception for connected and autonomous vehicles** [[paper]](https://ieeexplore.ieee.org/document/10646529)
- (TIV'16) **A Survey of Motion Planning and Control Techniques for Self-driving Urban Vehicles** [[paper]](https://ieeexplore.ieee.org/document/7490340)
- (Access'20) **V2x support in 3gpp specifications: From 4g to 5g and beyond** [[paper]](https://ieeexplore.ieee.org/document/9212349)
- (MONET'21) **Vehicular Edge Computing and Networking: A Survey** [[paper]](https://dl.acm.org/doi/10.1007/s11036-020-01624-1)
- (ASPLOS'17) **Neurosurgeon: Collaborative intelligence between the cloud and mobile edge** [[paper]](https://dl.acm.org/doi/10.1145/3037697.3037698)
- (Netw.'20) **Security and privacy challenges in 5g-enabled vehicular networks** [[paper]](https://ieeexplore.ieee.org/document/9055735)
- (ECVA'23) **Drivelm: Driving with graph visual question answering** [[paper]](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/06870.pdf)
- (aXiv'23) **Universal and transferable adversarial attacks on aligned language models** [[paper]](https://arxiv.org/abs/2307.15043)


### Intelligent Healthcare:
 Assisting clinicians in local diagnostic reasoning and patient monitoring, mitigating the privacy risks of centralized cloud inference for highly sensitive patient medical records.
- (Proc. IEEE'24) **Edge intelligence: Paving the last mile of artificial intelligence with edge computing**[[paper]](https://ieeexplore.ieee.org/document/8736011)
- (COMST'25) **Mobile edge intelligence for large language models: A contemporary survey**[[paper]](https://ieeexplore.ieee.org/document/10835069)
- (ICLR'17) **Outrageously large neural networks: The sparsely-gated mixture-of-experts layer** [[paper]](https://openreview.net/forum?id=B1ckMDqlg)
- (TMI'23) **Lvit: language meets vision transformer in medical image segmentation** [[paper]](https://ieeexplore.ieee.org/document/10172039)
- (Nature'23) **Large language models encode clinical knowledge** [[paper]](https://www.nature.com/articles/s41586-023-06291-2)
- (ETT'22) **Edge computing in smart health care systems: Review, challenges, and research directions** [[paper]](https://dl.acm.org/doi/abs/10.1002/ett.3710)
- (S&P'24) **Gpu. zip: On the side-channel implications of hardware-based graphical data compression** [[paper]](https://ieeexplore.ieee.org/document/10646718)



### Embodied Robotics: 
Operating in smart factories and humanoid platforms with strict 10-100 ms end-to-end latency requirements, reducing massive communication bandwidth overheads while interacting with physical environments.
- (COMST'25) **Mobile edge intelligence for large language models: A contemporary survey**[[paper]](https://ieeexplore.ieee.org/document/10835069)
- (ICML'22) **GLaM: Efficient scaling of language models with mixtureof-experts** [[paper]](https://icml.cc/media/icml-2022/Slides/17378.pdf)
- (aXiv'24) **OpenVLA: An Open-Source Vision-Language-Action Model** [[paper]](https://arxiv.org/abs/2406.09246)
- (CUI'23) **Harnessing Large Language Models for Cognitive Assistants in Factories** [[paper]](https://dl.acm.org/doi/10.1145/3571884.3604313)
- (TS 23.401) **3rd generation partnership project; technical specification group services and system aspects; general packet radio service (gprs) enhancements for evolved universal terrestrial radio access network (e-utran) access** [[paper]](https://portal.3gpp.org/desktopmodules/Specifications/SpecificationDetails.aspx?specificationId=849)
- (IPC'09) **The case for vm-based cloudlets in mobile computing** [[paper]](https://ieeexplore.ieee.org/document/5280678)
- (TWC'19) **Edge ai: On-demand accelerating deep neural network inference via edge computing** [[paper]](https://ieeexplore.ieee.org/document/8876870)
- (TII'19) **Sparse feature learning for correlation filter tracking toward 5g-enabled tactile internet** [[paper]](https://ieeexplore.ieee.org/document/8669788)
- (PIEEE'19) **Edge computing for autonomous driving: Opportunities and challenges** [[paper]](https://ieeexplore.ieee.org/document/8744265)
- (PMLR'17) **Communication-efficient learning of deep networks from decentralized data** [[paper]](https://proceedings.mlr.press/v54/mcmahan17a/mcmahan17a.pdf)
- (PMLR'23) **Rt-2: Vision-language-action models transfer web knowledge to robotic control** [[paper]](https://proceedings.mlr.press/v229/zitkovich23a.html)
- (aXiv'23) **VoxPoser: Composable 3D Value Maps for Robotic Manipulation with Language Models** [[paper]](https://arxiv.org/abs/2307.05973)



---

## 📃 Citation

```bibtex
@article{mo2025edge,
  title={Edge MoE: A Survey of Optimization Strategies for Mixture-of-Experts LLMs on the Edge},
  author={Mo, Zhenjia and Zhao, Yong and He, Qiang and Zhang, Mingjin and Chen, Yicong and Li, Ruitao and Qiu, Zihao and Wen, Hao and Chen, Shengyuan and Zhang, Qinggang and Ren, Wei and Cao, Jiannong},
  journal={arXiv preprint},
  year={2025}
}
