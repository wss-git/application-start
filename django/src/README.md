# 写在前头

注意：
1. 启动端口一定要和 caPort 配置端口一致，caPort 默认是 9000
2. 启动不要使用127.0.0.1 要使用、使用、用[0.0.0.0](https://help.aliyun.com/document_detail/132044.html#title-gor-w3v-hee) 启动


# 部署

1. 将 s.yml 里面的 Access 修改为自己的密钥别名
2. 确认环境
- 当前机器存在 python3 环境和 pip3 可直接执行 s deploy
- 当前有 docker 环境可将 s.yml 里面的 Hook: pip3 install -t ./tmp -r requirements.txt 修改为 Hook: s build docker
3. 执行 s deploy

# DockerFile

使用镜像的文件