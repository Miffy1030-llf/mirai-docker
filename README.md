# Mirai-docker

> 本项目使用 openjdk11 docker 镜像封装了 `mirai-2.3.2` 和 `mirai-api-http-1.9.8` 方便使用

## 首次使用说明

1. 首先确定安装好 docker 以及 docker-compose 并克隆该仓库

2. 运行 `prepare.sh` 下载 `mirai` 相关文件

3. `docker-compose up -d` 然后 `docker-compose down` 使程序文件结构初始化

4. 修改 `docker-compose.yml` 文件中 `environment` 的各个参数

5. `docker-compose up -d` 运行程序

6. `docker attach miraidocker_mirai_1` 进入控制台，按提示通过验证
    >项目文件夹下的 `tmp` 文件夹即为验证码保存的图片文件夹

## 注意

推荐先在服务器所在 IP 登录 PC 版 QQ 一个星期左右再使用 mirai 登录，并且将登录成功得到的   `device.json` 妥善保存