# 基于多模态AI大模型的全息媒体创意
该项目提供了一个简化且用户友好的平台，简化了高质量视频生成的复杂性。

## 环境搭建
在Ubuntu 24.04上进行测试。

1. 基础软件安装
安装`docker`：
```shell
sudo apt-get install docker.io
```
将普通用户加到docker组里：
```shell
sudo apasswd -a $USER docker
```
更新docker组
```shell
newgrp docker
```

2. 安装

克隆仓库：
```shell
https://github.com/OpenHUTB/holography.git
cd holography
```

构建镜像：
```shell
docker build -t opensora .
```

以交互模式启动docker容器：
```shell
docker run -ti --gpus all -v .:/workspace/Open-Sora opensora
```

## 参考
* [Open-Sora 技术报告](https://github.com/hpcaitech/Open-Sora/blob/main/docs/zh_CN/report_v3.md) 