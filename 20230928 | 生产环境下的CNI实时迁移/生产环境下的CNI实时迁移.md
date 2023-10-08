生产环境下的CNI实时迁移 | Live CNI Migration in Production Environments - Yike Wang and Yanzhao Li, VMware

https://kccncosschn2023.sched.com/event/1RTBY/chang-hou-zha-cnihui-zhe-live-cni-migration-in-production-environments-yike-wang-and-yanzhao-li-vmware

CNI（容器网络接口）负责设置集群Pod网络，一些更全面的CNI解决方案还可以设置高级网络功能，如网络策略和kube-proxy替代。CNI Pod网络是L4服务和L7入口网络的基础。我们的客户希望将现有集群切换到另一个CNI，并且我们经常收到这样的客户请求。 在这个会话中，我们将介绍： 
集群网络基础知识和CNI基础知识。
为什么在生产环境中总是需要进行CNI迁移，以及Tanzu项目如何管理多个CNI解决方案。
在现有集群上进行基本的CNI迁移方法以及在过程中对集群网络，包括Pod网络、L4服务和L7入口的停机时间的分析。
两种改进的方法，以克服流量停机时间，实现实时迁移。
我们在帮助客户在大规模集群中迁移CNI时所学到的经验教训。

CNI(container networking interface) is responsible for setting up cluster pod networking, and some more comprehensive CNI solutions can also set up advanced networking features such as network policy and kube-proxy replacement. The CNI Pod networking is the basis for L4 service and L7 ingress networking. Our customers want to switch to another CNI for their existing clusters and we see such requests from customers a lot. In this session, we’ll Introduce: 
Cluster networking basics and CNI basics
Why CNI migration is always needed in the production environment, and how the Tanzu project manages multi CNI solutions.
The basic in-place CNI migration method on an existing cluster and the analysis of the downtime on cluster networking including pod networking, L4 service and L7 ingress during the process.
Two improved methods to overcome the traffic downtime to implement live migration.
The lessons we learned when helping customers migrate CNI in large scale cluster