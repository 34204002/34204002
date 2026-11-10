# Jiang_I

南昌大学计算机专业，写 Java 后端。

仓库里的项目基本都是我一个人从需求、数据库设计一路写到前后端的，都能跑起来。最近在折腾 Spring AI，把 RAG、Agent、工具调用接进传统的 Spring Boot 系统里，让老业务听懂人话。Neo4j 也玩了一阵，关系一多、纸上画不清的时候，几行 Cypher 反而讲得明白。

## 现在在做的

一份长期记忆系统的设计草案，v0.1，供讨论，尚未实施。想做的是有稳定角色设定、能记住共同经历的聊天伙伴。跟知识库助手是两个独立项目，会新建仓库，原来的保留。

第一版只做记忆连续性。判断做没做成看五件事：跨会话记住明确偏好、换个说法能找回相关经历、用户更正后采用新信息、不把猜测和角色扮演写成真实经历、无关的时候不翻旧账。复杂情绪模拟、自主目标、主动联系用户这些都不在第一版里。

实施分四阶段，第一阶段先修会话连续性：Redis 失效后从 MySQL 恢复近期原文、话题状态设长度上限、用统一 token 预算代替无限累计的摘要。

记忆分三层，原始记录、整理后的认识、检索索引。原始记录留在 MySQL，Qdrant 只用来查。模型整理会出错，所以每条记忆要能看见出处、能改、能删、能重建。

## 已经做完的

- [jiang_I-agent](https://github.com/34204002/jiang_I-agent) 个人 AI 知识库助手。Spring Boot 4.1 + Spring AI 2.0 + DeepSeek，前端 Vue 3；RAG 向量 + Neo4j 知识图谱双检索，19 个 @Tool 工具方法，SSE 流式输出。[演示视频（B站）](https://www.bilibili.com/video/BV17F7W6GEnM/)
- [AI_Native_TakeOut](https://github.com/34204002/AI_Native_TakeOut) 外卖全流程平台，五处 AI 增强；AI 超时 500ms 自动降级，不影响下单。
- [DianPing](https://github.com/34204002/DianPing) 本地生活平台，Redis Lua 原子扣减 + RabbitMQ 异步下单；JMeter 实测 200 并发抢 100 单、零超卖。
- [BBS_Forum](https://github.com/34204002/BBS_Forum) 南昌大学校园 BBS，从需求、接口文档到部署上线，在云服务器上跑过一版。
- [LeetCode_myself](https://github.com/34204002/LeetCode_myself) 刷题记录。

## 其他

邮箱 [34204002@qq.com](mailto:34204002@qq.com)。
