
配置说明
```
port 6379
daemonize yes
pidfile /var/run/redis.pid

#指定数据文件存放位置，必须要指定不同的目录位置，不然会丢失数据
dir ./
#启动集群模式
cluster-enabled yes
#集群节点信息文件
cluster-config-file nodes-6379.conf
# 节点离线的超时时间
cluster-node-timeout 5000
#去掉bind绑定访问ip信息
#bind 127.0.0.1
#关闭保护模式
protected-mode no 
#启动AOF文件
appendonly yes
requirepass 123456
#设置集群节点间访问密码，跟上面一致
masterauth 123456
```