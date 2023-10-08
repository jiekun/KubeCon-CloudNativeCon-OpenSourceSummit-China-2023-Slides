在Kubernetes上构建一个精细化和智能化的资源管理系统 | Building a Fine-Grained and Intelligent Resource Management System on Kubernetes - He Cao & Wei Shao, ByteDance

https://kccncosschn2023.sched.com/event/1RSk1/nanokubernetesken-yong-rexia-zha-pian-fa-lia-xu-ni-building-a-fine-grained-and-intelligent-resource-management-system-on-kubernetes-he-cao-wei-shao-bytedance

原生 Kubernetes 的资源管理能力有所局限：1. 静态的资源模型会导致节点的资源利用率较低，因为在线业务具有潮汐现象。2. 只支持申请整数个 GPU，在 AI 推理场景下会浪费大量昂贵的 GPU 资源。3. 原生的拓扑亲和策略只考虑了 NUMA 拓扑，难以满足搜索、推荐和 AI 大模型训练等业务对性能的要求。 
在本次演讲中，曹贺和邵伟将介绍资源管理系统 Katalyst 及其在字节跳动的应用：1. 通过在离线混部提升资源利用率，并保障业务的 SLO 不受影响。2. 实现了 GPU 共享调度，支持 1% 算力粒度和 1 MiB 显存粒度的容器调度，从而提升了 AI 推理场景下的 GPU 利用率。3. 实现了拓扑感知调度，并扩展了 GPU 和 RDMA 在 PCIe Switch 级别的亲和策略，从而在分布式模型训练场景下可以使用 GPU DirectRDMA 技术来提升训练速度。4. 通过在线超分、规格推荐、潮汐混部等低使用门槛的措施提升资源效能。 
The resource management capabilities of vanilla Kubernetes are limited: 
The static resource model leads to low resource utilization due to the tidal nature of online services. 
Only full GPU requests are allowed, which causes huge GPU waste in AI inference scenarios. 
The native micro-topology allocation strategy can not meet the performance requirements of workloads such as search, recommendation, and large model training.
In this talk, He and Wei will introduce a resource management system, Katalyst, and its application in ByteDance: 
Colocate online services and offline jobs to improve resource utilization and ensure their SLOs. 
Implement GPU-sharing scheduling, which allows requests of 1% granularity computing power and 1 MiB granularity GPU memory, to improve GPU utilization in AI inference scenarios. 
Implement topology-aware scheduling and customize a strategy for GPU-RDMA affinity at the PCIe switch level, so GPUDirect RDMA can be used to accelerate distributed model training.
Enhance resource efficiency through easily implementable methods such as node over-commitment, specification recommendation, and tidal colocation.