如何加速模型训练并消除云计算中的I/O瓶颈 | How to Accelerate Model Training and Eliminate the I/O bottleneck for the Cloud - Rui Su, Juicedata

https://kccncosschn2023.sched.com/event/1RSee/fu-nfxiao-zhen-mang-dou-zhao-zha-iomin-ao-how-to-accelerate-model-training-and-eliminate-the-io-bottleneck-for-the-cloud-rui-su-juicedata

人工智能训练需要大量的数据，导致存储成本不断增加。由于其可扩展性和成本效益，对象存储备受关注。然而，直接使用它会带来某些挑战，包括低元数据性能、缺乏原子重命名操作和最终一致性问题。这些挑战在模型训练阶段尤为明显。 
同时，容器化技术正在流行。然而，传统的分布式文件系统缺乏横向扩展性，这使得难以支持 Kubernetes 的广泛可扩展性。另外，由于计算不再局限于一组固定的机器，数据需要智能地随着计算资源的移动而“流动”。 
我们旨在分享我们的实际经验。我们将探讨如何在保持上层组件不变的情况下，优化存储层的I/O效率，包括数据缓存、预取、并发读取和调度。 
AI training requires vast amounts of data, resulting in increasing storage costs. Object storage has gained attention due to its scalability and cost-effectiveness. However, direct usage of it brings certain challenges, including low metadata performance, lack of atomic rename operations, and eventual consistency issues. These challenges are particularly pronounced during the model training phase. 
Simultaneously, containerization technology is trending. However, traditional distributed file systems lack horizontal scalability, making it difficult to support the extensive scalability of Kubernetes. Additionally, as computing is no longer limited to a fixed set of machines, data needs to intelligently "flow" with the movement of computational resources. 
We aim to share our practical experience. We will explore how to optimize the storage layer's I/O efficiency in data caching, prefetching, concurrent reads, and scheduling while keeping the upper-layer components unchanged.