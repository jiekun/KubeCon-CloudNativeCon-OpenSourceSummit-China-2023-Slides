如何在大型集群中加速 Pod 的启动？ | How Can Pod Start-up Be Accelerated on Nodes in Large Clusters? - Paco Xu, DaoCloud & Byron Wang, Birentech

https://kccncosschn2023.sched.com/event/1PTFR/nanonfzhong-shi-fu-pod-zha-dyags-how-can-pod-start-up-be-accelerated-on-nodes-in-large-clusters-paco-xu-daocloud-byron-wang-birentech

这个想法来自我最近写的博客  Kubernetes 1.27：加速Pod启动的更新。 这是一个集群管理员可能面临的常见问题。 本次会话将向您展示Pod启动的过程以及如何加速Pod的启动。 

API：  控制器管理器创建Pod的时间，  KCM：PV和PVC绑定以及Webhooks。 
                                  
                                
调度：  GPU拓扑感知，节点负载感知。
                                
来自kubelet方面的节点级别：  镜像拉取，Sidecar，API QPS和Burs，事件驱动PLEG，  限流，磁盘和卷驱动程序，静态CPU策略，容器运行时。
                                  
                                
GPU管理：  拓扑不仅仅是NUMA，共享和监控。
                                
数据负载：  数据预加载和本地存储或分布式存储。
                                
可观察性：  如何检查为什么Pod启动缓慢？
                                
The idea came from my recently written blog Kubernetes 1.27: updates on speeding up Pod startup. This is a common issue that cluster administrators may face. This session will show you the process of pod startup and everything about how to speed up the startup of pods. 

API:  the creation time of pods by controller-manager,  KCM: PV & PVC binding and webhooks. 
                                  
                                
Scheduling:  GPU Topology-aware, node load aware 
                                
Node level from the kubelet side:  Image Pulling, Sidecar, API QPS & Burs, Event-Driven PLEG, Throttling, Disk and Volume driver, Static CPU Policy, Container Runtime 
                                
GPU Management:  Topology not only NUMA, Sharing, and Monitoring 
                                
Data load:  data preload & local storage or distributed storage 
                                
Observability:  How to check why the pod starts up slowly?