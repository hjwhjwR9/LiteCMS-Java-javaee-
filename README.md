# LiteCMS-Java-javaee-
LiteCMS-Java：基于 Spring Boot 3 + Vue 3 的轻量级内容管理系统。采用前后端分离架构，集成 MyBatis-Plus 与 Element Plus，代码分层清晰（Controller/Service/Mapper）。适合作为 Java EE 课程设计、毕业设计参考或企业级后台管理系统的二次开发脚手架   



🚀 LiteCMS-Java

基于 Spring Boot + Vue 3 的轻量级企业级内容管理系统
✨ 前后端分离 | 🛠️ 代码规范 | 🎓 适合实训/毕设/二开

📖 项目简介

LiteCMS-Java 是一套现代化的 Java 全栈 CMS 解决方案。本项目旨在提供一个架构清晰、易于扩展的内容管理平台。

系统采用主流的 前后端分离 架构：
后端：基于 Spring Boot，集成 MyBatis-Plus，提供高性能 RESTful API。
前端：基于 Vue 3 + Vite + Element Plus，界面美观，交互流畅。

无论是作为 Java EE 课程设计、毕业设计参考，还是作为 企业内部后台管理系统的脚手架，LiteCMS-Java 都是你的理想选择。

✨ 核心功能

📊 数据看板：可视化展示文章统计、用户增长及系统负载情况。
📝 文章管理：支持富文本编辑（Markdown/HTML）、分类标签管理、封面图上传。
🔐 权限控制 (RBAC)：基于角色的权限管理，精确控制菜单访问与按钮操作权限。
💬 互动评论：内置评论审核机制，支持敏感词过滤。
⚙️ 系统设置：网站基础信息配置、轮播图管理、操作日志审计。

🛠️ 技术栈
模块   技术选型   备注
前端   Vue 3, Vite, Element Plus, Pinia   组合式 API，响应式状态管理

后端   Spring Boot, MyBatis-Plus   简化 SQL 开发，快速构建

数据库   MySQL 5.7 / 8.0   关系型数据存储

工具   Maven, Lombok, Swagger/Knife4j   依赖管理与接口文档

📂 目录结构

为了保持代码整洁，本项目将前后端代码物理隔离：

LiteCMS-Java
├── backend/          # 🟢 后端工程 (Spring Boot)
│   ├── src/main/java # Java 源码 (Controller, Service, Mapper)
│   ├── src/main/resources # 配置文件 (application.yml)
│   └── pom.xml       # Maven 依赖管理
├── frontend/         # 🔵 前端工程 (Vue 3)
│   ├── src/          # 页面组件、路由、API 请求
│   ├── public/       # 静态资源
│   └── package.json  # Node 依赖管理
└── README.md         # 项目说明文档

⚙️ 环境准备

在开始运行之前，请确保你的电脑已安装以下环境（版本非常重要）：

JDK: 17+ (推荐) 或 1.8+
   注：若使用 Spring Boot 3.x 必须 JDK 17+
Maven: 3.6+
Node.js: 16.0+ (强烈建议 18+)
   注：Vite 构建工具对 Node 版本有要求，过低会报错
MySQL: 5.7 或 8.0

🏃‍♂️ 快速启动

数据库初始化
在 MySQL 中创建一个名为 lite_cms 的数据库，并导入 backend/src/main/resources/sql/init.sql 文件。

启动后端
进入 backend 目录，修改 application.yml 中的数据库账号密码，然后运行：
mvn spring-boot:run
或者在 IDE 中运行 Application.java 主类

后端默认端口：8080

启动前端
进入 frontend 目录，安装依赖并启动：
npm install
npm run dev


📸 项目截图
![输入图片说明](%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202026-07-01%20160057.png)

🤝 贡献与联系

欢迎提交 Issue 或 Pull Request！
作者：2774819989
邮箱：2774819889@qq.com

📄 开源协议

本项目基于 MIT 协议开源，您可以自由使用和修改。

这份 README 已经可以直接使用了。如果你需要补充具体的“数据库表结构设计”或者“API接口文档链接”，随时告诉我，我帮你加进去！
