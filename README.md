# northstar
北极星(NorthStar) 大数据中台

## 项目介绍
北极星(NorthStar) 大数据中台产品，旨在帮助企业用户快速收集, 整理数据及构建数仓, 且可进行数据服务及数据资产管理。
### 主要特色
- 快速构建数据模型
- 任务建模流程化
- 数据清洗: 模块化流程式
- 权限: 基于标签的权限形式,可快速为中台人员定制权限
- 数据质量: 自由定义质量规则及快速检测判定数据质量
- 数据知识: 基于用于业务自由定义业务元数据, 为企业积累数据知识
- 多种任务触发形式: 即可基于周期反复触发中台任务执行,也可基于业务进度实时触发中台任务执行

### 项目页面预览
#### 后台管理系统
登陆页
![登陆页](https://northstarbdg.github.io/northstar/%E9%A1%B9%E7%9B%AE%E9%A2%84%E8%A7%88/%E7%99%BB%E9%99%86.png)

概述页
![概述页](https://northstarbdg.github.io/northstar/%E9%A1%B9%E7%9B%AE%E9%A2%84%E8%A7%88/%E6%A6%82%E8%BF%B0.png)

数仓管理
![数仓管理](https://northstarbdg.github.io/northstar/%E9%A1%B9%E7%9B%AE%E9%A2%84%E8%A7%88/%E6%95%B0%E4%BB%93%E7%AE%A1%E7%90%86.png)

## 技术特性
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
| TIDB                 | 数据库             | https://www.pingcap.com/              |
| Nginx                | 静态资源服务器      | https://www.nginx.com/                         |
| Druid                | 数据库连接池        | https://github.com/alibaba/druid               |   |
| JWT                  | JWT登录支持         | https://github.com/jwtk/jjwt                   |
| Lombok               | 简化对象封装工具    | https://github.com/rzwitserloot/lombok         |
| Hutool               | Java工具类库        | https://github.com/looly/hutool                |
| PageHelper           | MyBatis物理分页插件 | http://git.oschina.net/free/Mybatis_PageHelper |
| Swagger-UI           | 文档生成工具        | https://github.com/swagger-api/swagger-ui      |
| Hibernator-Validator | 验证框架            | http://hibernate.org/validator                 |

#### 前端技术

| 技术       | 说明                   | 官网                                    |
| ---------- | --------------------- | -------------------------------------- |
| Vue        | 前端框架               | https://vuejs.org/                     |
| Vue-router | 路由框架               | https://router.vuejs.org/              |
| Pinia      | 全局状态管理框架        | https://pinia.vuejs.org/               |
| ElementPlus| 前端UI框架             | https://element-plus.gitee.io/         |
| Axios      | 前端HTTP框架           | https://github.com/axios/axios         |
| Echarts    | Echarts的图表框架      | https://echarts.apache.org/             |
| ChunkUI    | 高级UI工具             | https://www.npmjs.com/package/chunk-ui |
| CodeMirror | 在线代码编辑器          | https://codemirror.net/                |

#### 架构图

##### 系统架构图

![系统架构图](https://northstarbdg.github.io/northstar/%E6%9E%B6%E6%9E%84%E5%9B%BE%E7%89%87.png)


#### 模块介绍

## 沟通交流

![沟通交流群](https://northstarbdg.github.io/northstar/%E6%B2%9F%E9%80%9A%E4%BA%A4%E6%B5%81%E7%BE%A4.png)
