# 基于SpringBoot+Vue的少儿编程管理系统

![Spring Boot](https://img.shields.io/badge/-Spring%20Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white) ![Vue3](https://img.shields.io/badge/-Vue3-grey?style=flat-square) ![MySQL](https://img.shields.io/badge/-MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![MyBatis](https://img.shields.io/badge/-MyBatis-000000?style=flat-square&logo=mybatis&logoColor=white) 

## 项目介绍

本系统是一款面向少儿编程培训机构的数字化教学与运营平台，针对课程体系分散、试听跟进靠表格、作业批改与打卡激励割裂、作品展示与考级报名缺少统一入口、家长难以及时掌握学习进度与积分成长等问题，把课程选课、试听跟进、作品展厅、作业打卡、考级赛事、积分商城、资讯科普与 AI 编程答疑整合到同一套前后端分离工程中。

系统采用 SpringBoot + Vue 架构，区分学员/家长、授课教师与系统管理员：学员端完成选课试听、作品发布、作业打卡、赛事报名、积分兑换与 AI 答疑；教师与管理员在文教中台维护课程班级、审核试听与作品、布置批改作业、发布赛事资讯、管理商城发货，并在 ECharts 看板查看报课趋势与作品热度。适合作为毕设、课设与少儿编程教培数字化学习参考。

## 主要功能模块

- **用户认证与三角色分流**：学员/家长、教师、管理员统一登录注册，JWT 鉴权；登录后按角色进入门户或文教中台，/admin 路由与接口双重隔离
- **门户首页大厅**：Banner 轮播、精选课程、优秀作品、考级与资讯速递，导流至各业务栏目
- **编程课程与选课试听**：按 Scratch/Python/C++/创客分类与难度筛选，查看大纲后选课报班或预约免费试听
- **少儿作品秀**：分类浏览作品、点赞评论、发布封面与工程文件；审核通过后展示并奖励成长积分
- **考级与赛事报名**：浏览等级考/创意赛/信奥认证，在线报名生成准考证，学习中心查看成绩奖项
- **积分商城兑换**：打卡与作品积累积分，兑换礼品并填写收货信息，跟踪发货签收
- **编程资讯与 AI 小导师**：阅读获奖喜报与科普文章；对话式答疑 Scratch/Python/C++ 入门问题
- **学习中心**：我的班级课表、课后作业提交、每日打卡领积分、我的赛事与兑换订单集中管理
- **经营数据看板**：报课趋势、分类占比、作品热度等 KPI，ECharts 图表辅助教务决策
- **教学与排课中台**：课程分类、课程上下架、班级排课、报课订单与试听审核跟进
- **作业打卡与作品审核**：任务布置批改打分、打卡流水、作品精选与评论管理
- **论文与 UML 概览**：配套论文设计实现页拼图与 UML 图列表，便于答辩材料对照

## 技术架构

- **后端**：Spring Boot + MyBatis-Plus + JWT + Lombok
- **前端**：Vue 3 + TypeScript + Vue Router + Pinia + Element Plus + Vite + ECharts
- **数据库**：MySQL

<!-- screenshots-start -->
## 系统截图

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/kidscode/%E7%99%BB%E5%BD%95%E9%A1%B5%E9%9D%A2.png" alt="登录页面" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/kidscode/%E7%94%A8%E6%88%B7%E9%A6%96%E9%A1%B5.png" alt="用户首页" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/kidscode/%E7%BC%96%E7%A8%8B%E8%AF%BE%E7%A8%8B.png" alt="编程课程" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/kidscode/%E5%AD%A6%E4%B9%A0%E4%B8%AD%E5%BF%83.png" alt="学习中心" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/kidscode/%E5%B0%91%E5%84%BF%E4%BD%9C%E5%93%81%E7%A7%80.png" alt="少儿作品秀" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/kidscode/%E7%A7%AF%E5%88%86%E5%95%86%E5%9F%8E.png" alt="积分商城" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/kidscode/%E7%AE%A1%E7%90%86%E5%91%98%E4%BB%AA%E8%A1%A8%E7%9B%98.png" alt="管理员仪表盘" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/kidscode/%E5%B0%91%E5%84%BF%E8%AF%BE%E7%A8%8B%E7%AE%A1%E7%90%86.png" alt="少儿课程管理" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/kidscode/%E8%AE%BA%E6%96%87%E5%9B%BE1.png" alt="论文图1" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/kidscode/%E8%AE%BA%E6%96%87%E5%9B%BE2.png" alt="论文图2" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/kidscode/UML%E5%9B%BE%E5%88%97%E8%A1%A8.png" alt="UML图列表" width="600" />

<!-- screenshots-end -->

## 接毕业设计和论文

### 作者微信：vvsgxmn  (支持修改、 部署调试、 支持代做毕设)

### 接网站建设、小程序

### 选题+开题报告+任务书+程序定制+安装调试+论文+答辩ppt 都可以做

### 购买地址：[https://www.vvxx.love](https://www.vvxx.love)（vv毕设网）

### 支持 **一键生成 UML 图**：上传项目压缩包即可自动产出功能模块图、用例图、流程图、E-R 图、时序图等全套毕设图表。

### 提供 **免费配套软件下载 + 安装说明 + 部署教程**

![vv毕设网 - 一键画图](https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/uml-draw.png)

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/image-20260825133349317.png" alt="image-20260825133349317" />

⚠️ Bug添加微信**免费修复**，免费修复。其他平台的私信一律不管（微信方便发送文件）
