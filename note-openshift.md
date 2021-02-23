# Openshit 4.X 教程汇总

https://access.redhat.com/documentation/en-us/

https://blog.csdn.net/weixin_43902588/article/details/105060359


[万字长文，说透了 Openshift4 的安装过程！](https://cloud.tencent.com/developer/article/1640415)


https://github.com/noobaa

https://github.com/noobaa/noobaa-operator

OpenShift Container Platform有两种基本类型：Installer Provisioned Infrastructure (IPI) clusters和User Provisioned Infrastructure (UPI) clusters。

使用IPI集群，OpenShift管理集群的所有方面，包括操作系统本身,参见: https://access.redhat.com/documentation/en-us/openshift_container_platform/4.6/html-single/deploying_installer-provisioned_clusters_on_bare_metal/index

使用UPI集群，必须自己管理和维护集群资源，包括：control plane、compute machine、load balancer、networking、DNS等。
IPI目前仅支持AWS，UPI支持AWS、vSphere、Bare metal。

[OpenShift 4新特性](https://blog.csdn.net/weixin_33840661/article/details/92964796?ops_request_misc=%25257B%252522request%25255Fid%252522%25253A%252522161287468916780266216205%252522%25252C%252522scm%252522%25253A%25252220140713.130102334.pc%25255Fall.%252522%25257D&request_id=161287468916780266216205&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_v2~rank_v29-2-92964796.pc_search_result_before_js&utm_term=openshift+IPI%25E5%25AE%2589%25E8%25A3%2585)

[在vmware vsphere上采用IPI方式安装Redhat Openshift集群4.6的回顾整理记录](https://blog.csdn.net/oasisss/article/details/113753481?ops_request_misc=%25257B%252522request%25255Fid%252522%25253A%252522161287468916780266216205%252522%25252C%252522scm%252522%25253A%25252220140713.130102334.pc%25255Fall.%252522%25257D&request_id=161287468916780266216205&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~first_rank_v2~rank_v29-3-113753481.pc_search_result_before_js&utm_term=openshift+IPI%25E5%25AE%2589%25E8%25A3%2585)

[OpenShift Container Platform 4.x 兼容性矩阵](https://access.redhat.com/articles/4128421)

[openshift 4.X和k8s API配套关系](https://access.redhat.com/solutions/4870701), openshift 4.6 用的是k8s 1.19 

[一文读懂OpenShift总体架构设计](https://blog.csdn.net/M2l0ZgSsVc7r69eFdTj/article/details/105884957?utm_medium=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-2.control&depth_1-utm_source=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-2.control)

[Redhat container存储架构](https://access.redhat.com/documentation/en-us/red_hat_openshift_container_storage/4.6/html-single/planning_your_deployment/index)

## Rancher 

[Rancher 2.5 功能特性](https://wenku.baidu.com/view/09fe140e370cba1aa8114431b90d6c85ed3a883a.html?fr=search-1-income6-psrec1&fixfr=a3tumIHdL8aZ9Bmdup%2FXvQ%3D%3D)

[Rancher架构](https://rancher.com/docs/rancher/v2.x/en/overview/architecture/)

[Rancher Longhorn块存储](https://longhorn.io/docs/1.0.2/concepts/)

容器平台的存储，主要用file ,block， 对象存储使用较少 
参见[Block Storage, Object Storage, and File Systems: What They Mean for Containers](https://rancher.com/block-object-file-storage-containers/)


## vmware容器平台

https://wenku.baidu.com/view/4e7bced727fff705cc1755270722192e4536580e.html?fr=search-1-income5-psrec1&fixfr=gjnjpdkalNECXRD5M1xtLA%3D%3D


[kubevirt升级](https://kubevirt.io/labs/kubernetes/lab3)


3+1保障：高可用系统稳定性是如何炼成的？  https://www.sohu.com/a/447421277_612370?spm=smpc.author.fd-d.4.1612137881996MZQWNEl


https://blog.csdn.net/weixin_36106852/article/details/113022355?ops_request_misc=&request_id=&biz_id=102&utm_term=k8s%E6%BB%9A%E5%8A%A8%E5%8D%87%E7%BA%A7%E5%8E%9F%E7%90%86&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduweb~default-0-113022355.pc_search_result_before_js&spm=1018.2226.3001.4187



http://manpages.ubuntu.com/manpages/trusty/man8/bridge.8.html

# work

https://askubuntu.com/questions/11709/how-can-i-capture-network-traffic-of-a-single-process