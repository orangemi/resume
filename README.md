宓文捷
======

|||
|------|----------|
| 出生日期 | 1987年10月6日 |
| 所在城市 | 中国 上海 |
| Email | orangemiwj@gmail.com |
| 电 话 | +86 13661471260 |

|||
|------|----------|
| github | https://github.com/orangemi |
| blog | https://github.com/orangemi/orangemi.github.io/issues |

## 教育经历
**2006.9 - 2010.6** 同济大学 土木工程学院 结构工程系

## 工作经历
### 2015.8 - 现在 上海汇翼科技信息有限公司
高级后端工程师，架构师，2016年评选为年度优秀员工。

**通知系统优化**

原有通知系统会占用大量系统CPU和IO资源，超过一定QPS会造成系统整体奔溃。利用时间换空间思路，使用RabbitMQ，使通知系统有无限横向拓展能力，提高通知和推送吞吐量(单机100QPS)。服务接口简单功能强大，让第三方应用友好接入，架构上支持多种下游渠道，方便扩展。通知的tag模式支持用户多维度筛选，反选，在自由维度批量操作中响应迅速。后期发现RabbitMQ亦有瓶颈，支持队列模型降级处理，建立使用mongodb或其他数据库而使用http/websocke等通用协议的数据库队列。

**搜索系统重构**

原有系统只能利用几个简单条件搜索，还经常出现数据漏查漏写。经过探索[CQRS模式](https://blog.imxiaomi.com/5.html)，重建数据模型，使用nest字段实现不定列自由类型数据模型，在上亿条文档中按照指定权限范围和特定搜索条件返回数据结果。该系统还通过重刷机制保证漏写或出错情况下能够自我修复。设计实现[`TQL搜索语言`](https://orangemi.github.io/teambition-tql/tql.html)，简化搜索场景，提高搜索查全率和查准率。后期使用多租户隔离模型分shard存储用户数据，减少查询总量优化查询速度。最后探索使用Elasticsearch为数据库实现实时统计的通用服务。

**建立支付后台**

公司初期的财务系统不完备，导致很多收入无法利用线上系统统计记账，在联合销售，财务，售后等多部门重新树立业务模型，使用DDD(领域驱动设计)思路，明确业务边界，独自创建了一个支持收支分离，多产品发货的支付系统，支持财务收入提成计算，建立MRR，ARR计算模型，解决MRR计算尾差问题，解决公司财务报表和审计的数据基础问题。

**建立日志系统**

公司早期缺乏日志处理。加入公司后建立线上日志收集和展示，从elk, ehk一路升级至基于kafka实现的event-bus，深入了解kafka后，建立通过日志数据流(kafka-stream)建立监控防黑系统，业务上也建立了初步数据流模型。目前该系统每天处理上10亿级数据，为了更好的维护日志系统，开发一个能够监控kafka本身的系统，调优kafka处理流程。

**架构和其他**

解决公司重点难点技术问题:
- 推进公司Docker化，解决镜像包体过大，打包过程中权限溢出问题；解决CI/CD流程中部署k8s；
- 制作一个基于公司权限系统的解决方案能够使得任何资源可以受控访问，并将其[开源](https://github.com/orangemi/teambition-nginx-gateway)；
- 利用ssh穿透，优化客户私网环境下开发模式。
- 利用nodejs流模型，支持文件上传下载支持分片模式。
- 推进公司全技术人员参与技术交流和分享，提升公司内技术为本的开发氛围。

------
### 2014.8 - 2015.8 广州云游控股有限公司(Forgame) 

后端工程师 除游戏服务器框架及游戏主要逻辑外，建立分布式服务器框架 负责运维，搭建代码部署系统，后台管理工具，发布更新系统，建立数据采集系统，实时数据统计系统。创建BI查询系统，

------
### 2011.10 - 2014.7 上海慕和网络科技有限公司

后端工程师 负责游戏后端框架业务开发；成功帮助公司反黑客, 反外挂，DDos攻击；建立手游多渠道支付平台，接入20多家国内外支付平台；建立风控机制防黑卡，每月阻止黑卡退费20万美元。

------
### 2011.6 - 2011.9 上海客齐集信息技术有限公司(百姓网) 

市场部业务工程师 建立公司内部会议室预订系统；对发布页面优化：发布成功率65%提升至70%，建立产品优化模型。

------
### 2010.8 - 2011.4 北京江河幕墙股份有限公司

「上海华润外滩九里」幕墙项目管理，参与外墙石材幕墙和玻璃开启扇施工管理；「上海平安大厦」幕墙项目管理，参与外墙石材幕墙，玻璃幕墙施工管理。

## 编程技能
- 熟悉node.js 5年开发经验，熟悉业务常用内建库: http net stream
- 熟悉web开发，有较多中小型项目开发经验，熟悉了解vue, webpack, 略懂rxjs
- 熟悉http网络协议 8年开发经验
- 熟悉各类数据库和队列模型，熟悉优劣，包括mysql, mongodb, elasticsearch, redis, kafka，rabbitmq
- 熟悉DevOps技能，熟练docker, k8s, bash
- 了解网络安全，了解web黑客攻防技能
- 略懂java，golang，参与线上开源项目和公司相关技术栈开发
- 熟悉php 3年开发经验
- 了解架构知识，DDD开发思想，微服务开发，nodejs性能优化

## 其他
中文母语，英语读写流利(CET-6)，日语基本读写；喜欢重新造轮子，实践出真知。
