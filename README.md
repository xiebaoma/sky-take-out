# 北京理工大学食堂点餐

## 环境配置

### 后端

IDEA

maven

### 前端

nginx

### 数据库

MySQL

## 项目部署

### 1，克隆到本地

```
git clone https://github.com/xiebaoma/sky-take-out.git
```

### 2，配置数据库和阿里云OSS

用IDEA打开项目，在 application.yml 和 application-dev.yml中配置你自己的数据库和云存储

### 3，配置maven依赖

在pom.xml文件中可根据需要修改依赖的版本，修改好之后更新依赖

### 4，编译运行

由于你是克隆的项目，所以建议先编译maven工程，没有报错后再运行

### 5，打开服务端

进入nginx目录，打开命令行，输入

```
start nginx
```

在浏览器输入：

```
localhost:8800
```

一切正常的话你就可以进入服务端的网页

（注意：你可以修改nginx的配置文件，自定义端口......）
