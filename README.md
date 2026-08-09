# Jiang_I

南昌大学计算机专业，写 Java 后端。

最近在折腾 Spring AI——把 RAG、Agent、工具调用接进传统的 Spring Boot 系统里，让老业务听懂人话。Neo4j 也玩了一阵，关系一多、纸上画不清的时候，几行 Cypher 反而讲得明白。

仓库里的项目都是我一个人从需求、数据库设计一路写到前后端，全部能跑：有带完整前端和演示视频的 Agent，有 QPS 翻几倍的秒杀系统，也有跑在云服务器上的论坛。

> 不想只写 CRUD，所以给自己项目里塞 AI、塞高并发、塞图数据库。

---

## 项目

### I-Agent — 个人 AI 知识库助手

从零写的一个完整 Agent 产品：后端 Spring Boot 4.1 + Spring AI 2.0 + DeepSeek，前端 Vue 3，整套设计系统自己搭。

- 自研 `@Tool` 注解框架：注册 19 个工具让模型自主调度（待办、提醒、查知识库、概念图谱……），线程上下文跨线程传递也是自己管的
- SSE 流式输出，DeepSeek 的"思考"过程单独推送、前端打字机渲染，单轮首字响应 < 300ms
- 检索走 RAG 向量 + Neo4j 知识图谱双通道："学 Redis 之前要先学什么"这种带前置关系的问题，纯向量检索答不了
- 知识库、图谱按用户隔离，JWT 鉴权 + Bucket4j 限流，工程化做得很足

[▶ 演示视频（B站）](https://www.bilibili.com/video/BV17F7W6GEnM/) · [源码](https://github.com/34204002/jiang_I-agent)

### 其他项目

| 项目 | 做了什么 | 技术 |
| :--- | :--- | :--- |
| [SkyTakeOut](https://github.com/34204002/SkyTakeOut) | 外卖全流程平台 + 五块 AI 增强：订单备注自动解析（"不要辣、放门卫"→ 标签）、差评 RAG 起草回复、智能客服、营销文案生成、经营数据自然语言查询。Redis 多级缓存让接口 QPS 提升 340%，AI 超时 500ms 自动降级，不碰核心流程 | Spring Boot / Spring AI / Redis / WebSocket |
| [FoodiePulse](https://github.com/34204002/hm-dianping) | 本地生活平台：Redisson 锁 + RabbitMQ 削峰做秒杀，1000+ 并发零超卖、秒杀 QPS 1500+；Redis 多级缓存把商户查询从 200 提到 1000 QPS；自然语言搜店（Function Calling）；Neo4j 好友推荐 | Spring Boot / Redis / Neo4j / RabbitMQ |
| [BBS_Forum](https://github.com/34204002/BBS_Forum) | 南昌大学校园 BBS：Markdown 发帖、楼中楼评论、积分系统、后台管理。从需求、接口文档到部署上线全流程自己走完，在云服务器上正式跑过一版 | Spring Boot / MyBatis-Plus / MySQL |
| [LeetCode_myself](https://github.com/34204002/LeetCode_myself) | 记录自己刷过的一些题目 | Java |

---

## 技术栈

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat&logo=springboot&logoColor=white)
![Spring AI](https://img.shields.io/badge/Spring%20AI-6DB33F?style=flat&logo=spring&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)
![Neo4j](https://img.shields.io/badge/Neo4j-4581C3?style=flat&logo=neo4j&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-FC4E32?style=flat&logo=qdrant&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat&logo=rabbitmq&logoColor=white)
![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat&logo=vuedotjs&logoColor=white)

---

## 最近在搞

- Spring AI：给旧系统加 RAG，写自己的 agent
- 刷 LeetCode，题解都放[这个仓库](https://github.com/34204002/LeetCode_myself)里了

---

## 联系

- 邮箱：[34204002@qq.com](mailto:34204002@qq.com)
- GitHub：[34204002](https://github.com/34204002)
