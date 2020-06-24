# github-ci-template

### 说明

@see [Github Actions - 使用 SSH 远程连接服务器部署](https://laogen.site/github-actions/ssh-deploy/)

首先，通常需要提前在服务器上首次初始化部署你的项目；

### 使用

#### Github Secrets

在 Github Project 中添加以下 Secret.

> dev.yml

`DEV_SERVER_SSH_PRIV_KEY`: 访问 dev 服务器的私钥
`DEV_SERVER_IP`: 访问 dev 服务器的IP

> prod.yml

`PROD_SERVER_SSH_PRIV_KEY`: 访问 prod 服务器的私钥
`PROD_SERVER_IP`: 访问 prod 服务器的IP

#### Deploy Scripts

`deploy-dev.sh` 和 `deploy-prod.sh` 分别是 dev 和 prod 环境下的应用部署脚本，你需要为每个项目编写部署脚本；
