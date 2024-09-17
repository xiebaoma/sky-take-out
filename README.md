# 外卖点餐项目

## 环境配置

### 后端

IDEA

maven

### 前端

nginx

微信开发者工具

### 数据库

MySQL

Redis

## 本地运行

### 1，克隆到本地

```
git clone https://github.com/xiebaoma/sky-take-out.git
```

### 2，配置数据库

启动MySQL和Redis

进入Redis目录，在命令行输入：

```
redis-server.exe redis.windows.conf
```

建立MySQL数据库，导入databases中的sql文件

在 application.yml 和 application-dev.yml中配置你自己的数据库

### 3，配置阿里云OSS

在阿里云上准备好OSS

用IDEA打开项目，在 application.yml 和 application-dev.yml中配置你自己的云存储

### 4，配置maven依赖

在pom.xml文件中可根据需要修改依赖的版本，修改好之后更新依赖

### 5，申请小程序

在微信公众号平台按要求申请注册一个小程序，并获得微信支付相关的配置数据，然后修改配置文件

### 6，编译运行

由于你是克隆的项目，所以建议先编译maven工程，没有报错后再运行

### 接口（可选）

可以通过接口进行调试

进入接口文档，将.json文件导入测试接口的应用（比如YAPI）

也可以直接通过前后端联调进行测试

### 7，打开服务端

进入nginx目录，打开命令行，输入（不要直接点击nginx.exe)

```
start nginx
```

在浏览器输入：

```
localhost:8800
```

一切正常的话你就可以进入服务端的网页

（注意：你可以修改nginx的配置文件，自定义端口......）

### 8，打开微信小程序

在微信开发者工具中打开mp-weixin，直接编译

## 部署上线

### 1，配置云服务器

你的服务器上需要配置以下环境：

1，Java开发环境（JDK）

2，MySQL数据库（并导入数据）

3，Redis数据库

4，Nginx

### 2，部署项目

将项目中的配置文件修改，然后在IDEA中将项目打包成jar包，将jar包直接上传到服务器（很多厂商的服务器都可以一键上传）

在命令行输入：

```
java -jar sky-take-out.jar
```

### 注册域名（可选）

### 3，测试

先将你的服务器防火墙修改一下，打开相关的端口

在浏览器测试服务端控制台。

在微信开发者工具测试小程序，记得先在vendor.js文件中修改一下baseUrl的地址（大约在20500行左右的地方），是你服务器上Nginx的地址。

### 4，上传小程序代码，申请上线

