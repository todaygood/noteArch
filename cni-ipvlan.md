

一个适合 Kubernetes 的最佳网络互联方案
【编者的话】本文比较了几种 Kubernetes 联网方案，包括 Flannel（aws-vpc | host-gw | vxlan）和 IPvlan 。目前建议选择 flannel + host-gw 方案，没有特别依赖，性能也够用。一旦 flannel 支持 IPvlan （有自动化设置工具了），且 Linux 内核版本比较新，就可以采用 IPvlan 方案。


http://dockone.io/article/1115

http://machinezone.github.io/research/networking-solutions-for-kubernetes

[Kubernetes网络解决方案的比较](http://jiagoushi.pro/book/export/html/175)


[Kuberbetes-- kubernetes网络方案总结（一）](https://zhangchenchen.github.io/2017/12/12/kubernetes-network-summary-1/)



