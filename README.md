# kafka集群部署方法

部署前准备：
1. 部署服务器的ip
2. 可用的9093 9094 9095 2181端口
3. docker和docker-compose

## 修改docker-compose.yaml文件

修改文件中```      KAFKA_ADVERTISED_LISTENERS: PLAINTEXT://192.168.202.219:9093```的ip为服务器ip

## 启动服务

```shell
sudo docker-compose up -d
```

进入eagle即可查看kafka状态http://127.0.0.1:8048/ 用户名密码是admin/123456
