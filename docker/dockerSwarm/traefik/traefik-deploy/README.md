#### 启动swarm
docker swarm init
#### 生成manager节点加入的命令
docker swarm join-token manager
#### 节点添加标签
docker node update --label-add role=master <nodeName>
