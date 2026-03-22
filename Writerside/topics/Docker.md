# 005 Docker

## 安装 Docker {id="docker_1"}

```bash
sudo apt install docker.io
```

## Docker 命令免密码 {id="docker_2"}

 将当前用户添加到 docker 组，可免密码使用 docker 命令

```bash
sudo usermod -aG docker $USER
```

## Docker 服务管理

设置 Docker 服务开机自启动

```bash
sudo systemctl enable docker
```

## 重启系统

以上配置重启生效

## 检查

输入命令 `docker version` 正确输出如下

```
Client:
 Version:           28.2.2
 API version:       1.50
 Go version:        go1.23.1
 Git commit:        28.2.2-0ubuntu1~24.04.1
 Built:             Wed Sep 10 14:16:39 2025
 OS/Arch:           linux/amd64
 Context:           default

Server:
 Engine:
  Version:          28.2.2
  API version:      1.50 (minimum version 1.24)
  Go version:       go1.23.1
  Git commit:       28.2.2-0ubuntu1~24.04.1
  Built:            Wed Sep 10 14:16:39 2025
  OS/Arch:          linux/amd64
  Experimental:     false
 containerd:
  Version:          1.7.28
  GitCommit:        
 runc:
  Version:          1.3.3-0ubuntu1~24.04.3
  GitCommit:        
 docker-init:
  Version:          0.19.0
  GitCommit:        

```

