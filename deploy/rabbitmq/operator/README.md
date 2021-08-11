## 安装rabbitmq Operator
```
wget https://github.com/rabbitmq/cluster-operator/releases/latest/download/cluster-operator.yml
kubectl apply -f cluster-operator.yml
```

## 创建rabbitmq 集群
```
kubectl apply -f nfs-pv.yaml
kubectl apply -f rabbitmq-cluster.yaml
```
