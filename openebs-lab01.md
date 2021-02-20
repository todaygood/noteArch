# openEBS 

https://www.bookstack.cn/read/kubernetes-handbook/practice-openebs.md

## version 

https://github.com/openebs/openebs/releases/tag/v2.6.0


## deploy 

helm install stable/openebs --name openebs --namespace openebs



## doc

[官方文档](https://docs.openebs.io/)

[OpenEBS架构](https://docs.openebs.io/docs/next/architecture.html)

https://www.bookstack.cn/books/kubernetes-handbook-201910



为了使用普通用户，按照上面的提示执行：

mkdir -p $HOME/.kube
sudo cp -i /etc/kubernetes/admin.conf $HOME/.kube/config
sudo chown $(id -u):$(id -g) $HOME/.kube/config
此时如果遇到执行命令时报如下错误：

$ kubectl version
Client Version: version.Info{Major:"1", Minor:"9", GitVersion:"v1.9.2", GitCommit:"5fa2db2bd46ac79e5e00a4e6ed24191080aa463b", GitTreeState:"clean", BuildDate:"2018-01-18T10:09:24Z", GoVersion:"go1.9.2", Compiler:"gc", Platform:"linux/amd64"}
The connection to the server localhost:8080 was refused - did you specify the right host or port?
需要修改/etc/kubernetes/manifests/kube-apiserver.yaml文件，修改下列参数：

- --insecure-port=8080
默认是0不打开，修改为8080即可。




