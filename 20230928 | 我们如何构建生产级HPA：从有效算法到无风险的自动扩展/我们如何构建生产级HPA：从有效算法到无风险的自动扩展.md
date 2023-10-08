我们如何构建生产级HPA：从有效算法到无风险的自动扩展 | How We Build Production-Grade HPA: From Effective Algorithm to Risk-Free Autoscaling - Ziqiu Zhu & Yiru Guo, Ant Group

https://kccncosschn2023.sched.com/event/1Rfyo/chang-wa-hpadaepzhao-la-wu-zha-kek-how-we-build-production-grade-hpa-from-effective-algorithm-to-risk-free-autoscaling-ziqiu-zhu-yiru-guo-ant-group

你是否曾经发现，Kubernetes HPA（水平自动扩展）的内置算法对于具有复杂资源使用特性的真实工作负载来说不太有效？或者，你是否曾经担心激进的自动扩展过程会突然破坏你“脆弱”的生产系统？ 
在这个会话中，来自蚂蚁集团的工程师将披露他们构建生产级HPA的方法，该方法每年可以稳定地节省约100,000个CPU核心。这包括一种创新的“基于流量驱动”的副本预测算法，非常适用于受多个复杂流量模式影响的工作负载，以及独特的多阶段灰度扩展策略，可以极大地减轻自动扩展过程中的风险。 
此外，他们还将利用Kapacity，一款新开源的云原生容量解决方案，演示如何将上述方法实际应用于你的Kubernetes环境，而无需依赖特定的供应商功能，做到轻松自如。 
Have you ever found that Kubernetes HPA's built-in algorithm is less effective for real-world workloads with complicated resource usage characteristics? Or, have you ever worried that a radical autoscaling process would suddenly break your "fragile" production system? 
In this session, engineers from Ant Group will disclose their methodology for building production-grade HPA, which has been saving ~100k CPU cores yearly with high stability. This includes an innovative "traffic-driven" replica prediction algorithm, which is well adapted to workloads whose resource usage is affected by multiple complex traffic patterns, and a unique multi-stage gray scaling strategy that greatly mitigates risks during autoscaling. 
Furthermore, they will utilize Kapacity, a newly open-sourced cloud native capacity solution, to demonstrate how to practically apply the above methodology to any of your Kubernetes environments with ease, without relying on specific vendor features.