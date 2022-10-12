# northstar
北极星数据管理中台
## 前言

`北极星数据管理中台`项目致力于打造一个完整的大数据平台，采用现阶段流行技术实现。

## 项目文档


## 项目介绍

##特性
- 基于数据同步与计算引擎纯钧和实时计算引擎Flink，支持JSON模版配置任务，兼容Flink SQL语法；
- 支持分布式运行，支持flink-standalone、yarn-session、yarn-per job等多种提交方式；
- 支持Docker一键部署，支持K8S 部署运行；
- 支持多种异构数据源，可支持MySQL、Oracle、SQLServer、Hive、Kudu等20多种数据源的同步与计算；
- 易拓展，高灵活性，新拓展的数据源插件可以与现有数据源插件即时互通，插件开发者不需要关心其他插件的代码逻辑；
- 不仅仅支持全量同步，还支持增量同步、间隔轮训；
- 批流一体，不仅仅支持离线同步及计算，还兼容实时场景；
- 支持脏数据存储，并提供指标监控等；
- 配合checkpoint实现断点续传；
- 不仅仅支持同步DML数据，还支持Schema变更同步；

### 技术选型

#### 后端技术

| 技术                 | 说明                | 官网                                           |
| -------------------- | ------------------- | ---------------------------------------------- |
| SpringBoot           | 容器+MVC框架        | https://spring.io/projects/spring-boot         |
| SpringSecurity       | 认证和授权框架      | https://spring.io/projects/spring-security     |
| MyBatis              | ORM框架             | http://www.mybatis.org/mybatis-3/zh/index.html |
| Mybatis-Plus         | ORM框架            | https://baomidou.com/    |
| Maven                | 程序构建            | https://maven.apache.org/       |
| RabbitMQ             | 消息队列            | https://www.rabbitmq.com/                      |
| Redis                | 分布式缓存          | https://redis.io/                              |
| xxl-job              | 定时任务            | https://www.xuxueli.com/xxl-job                        |
| Chunjun              | 数据同步与计算       | https://dtstack.github.io/chunjun                        |
| Flink                | 实时计算引擎         | https://flink.apache.org/                       |
| xxl-job              | 定时任务            | https://www.xuxueli.com/xxl-job/                        |
| LogStash             | 日志收集工具        | https://github.com/elastic/logstash            |
| Kibana               | 日志可视化查看工具  | https://github.com/elastic/kibana              |
| Nginx                | 静态资源服务器      | https://www.nginx.com/                         |
| Docker               | 应用容器引擎        | https://www.docker.com                         |
| Jenkins              | 自动化部署工具      | https://github.com/jenkinsci/jenkins           |
| Druid                | 数据库连接池        | https://github.com/alibaba/druid               |   |
| JWT                  | JWT登录支持         | https://github.com/jwtk/jjwt                   |
| Lombok               | 简化对象封装工具    | https://github.com/rzwitserloot/lombok         |
| Hutool               | Java工具类库        | https://github.com/looly/hutool                |
| PageHelper           | MyBatis物理分页插件 | http://git.oschina.net/free/Mybatis_PageHelper |
| Swagger-UI           | 文档生成工具        | https://github.com/swagger-api/swagger-ui      |
| Hibernator-Validator | 验证框架            | http://hibernate.org/validator                 |

#### 前端技术

| 技术       | 说明                  | 官网                                   |
| ---------- | --------------------- | -------------------------------------- |
| Vue        | 前端框架              | https://vuejs.org/                     |
| Vue-router | 路由框架              | https://router.vuejs.org/              |
| Vuex       | 全局状态管理框架      | https://vuex.vuejs.org/                |
| Element    | 前端UI框架            | https://element.eleme.io               |
| Axios      | 前端HTTP框架          | https://github.com/axios/axios         |
| v-charts   | 基于Echarts的图表框架 | https://v-charts.js.org/               |
| Js-cookie  | cookie管理工具        | https://github.com/js-cookie/js-cookie |
| nprogress  | 进度条控件            | https://github.com/rstacruz/nprogress  |

#### 架构图

##### 系统架构图

![系统架构图](http://img.macrozheng.com/mall/project/mall_micro_service_arch.jpg)

##### 业务架构图

![系统架构图](http://img.macrozheng.com/mall/project/mall_business_arch.png)

#### 模块介绍
