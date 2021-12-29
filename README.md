# father-web

> 表情包网站 [爸爸](http://father.cool) 后端项目

## 技术栈

- Java 8
- 开发框架：SpringBoot 2.x
- 数据访问：MyBatis + MyBatis Plus
- 项目管理：Maven
- 接口文档：Swagger + Knife4j
- 数据库：MySQL
- 对象存储：Tencent COS

## 启动方法

1. 修改 resources 目录下的 application、application-prod 配置文件，把数据库地址改为自己的

2. 在 FatherBackendApplication 文件中，找到下列代码：

```java
@SpringBootApplication(exclude = {DataSourceAutoConfiguration.class})
```   

改为：

```java
@SpringBootApplication
```


2. 使用 [微信云托管](https://cloud.weixin.qq.com) 等容器平台，直接导入仓库代码，会自动读取 Dockerfile 进行镜像构建和发布