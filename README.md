# 使用 docker 搭建 jenkins 服务

## Usage

### 运行服务

```bash
docker-compose up -d
```

访问 <http://localhost:8080> 进入 jenkins 页面。

注意：首次进入 jenkins 页面时，需要进行一些设置，从 `home/secrets/initialAdminPassword` 文件中获取初始管理密码。

### 升级 jenkins

```bash
# 拉取最新镜像
docker pull jenkins/jenkins:lts-alpine

# 重启服务
docker-compose down
docker-compose up -d
```
