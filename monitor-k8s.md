# k8s监控方案
cadvisor+heapster+influxdb+grafana
缺点：只能支持监控容器资源，无法支持业务监控，扩展性较差

cadvisor/exporter+prometheus+grafana
总体流程: 数据采集-->汇总-->处理-->存储-->展示

1. 容器的监控
prometheus使用cadvisor采集容器监控指标，cadvisor集成在k8s的kubelet中-通过prometheus进程存储-使用grafana进行展现
node的监控-通过node_pxporter采集当前主机的资源-通过prometheus进程存储-使用grafana进行展现
master的监控-通过kube-state-metrics插件从k8s中获取到apiserver的相关数据-通过prometheus进程存储-使用grafana进行展现

2.kubernetes监控指标

kubernetes自身的监控

node的资源利用率-node节点上的cpu、内存、硬盘、链接
node的数量-node数量与资源利用率、业务负载的比例情况、成本、资源扩展的评估
pod的数量-当负载到一定程度时，node与pod的数量，评估负载到哪个阶段，大约需要多少服务器，每个pod的资源占用率如何，进行整体评估
资源对象状态-k8s在运行过程中，会创建很多pod，控制器，任务，这些内容都是由k8s中的资源对象进行维护，需要进行对资源对象的监控，获取资源对象的状态

pod监控
每个项目中pod的数量-正常的pod数量，有问题的pod数量
容器资源利用率-统计当前pod的资源利用率，统计pod中的容器资源利用率，cpu、网络、内存评估
应用程序-项目中的程序的自身情况，如并发，请求响应，项目用户数量，订单数等

作者：baiyongjie
链接：https://www.jianshu.com/p/e76053b6f3f5
来源：简书
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。
node exporter
收集各k8s node节点(master/node)上的监控指标数据，监听端口为9100

## 

[WeaveScope](https://www.yisu.com/zixun/7459.html)
