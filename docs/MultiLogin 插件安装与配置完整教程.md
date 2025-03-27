# MultiLogin 插件安装与配置完整教程

## 一、项目概述与技术架构

MultiLogin 是一款专为 Minecraft 服务器设计的创新插件，通过 Java 和 Kotlin 双语言开发，完美解决了正版验证与多种外置登录系统（如 AuthMe、Cracked 等）的兼容问题。该插件支持 Bukkit、BungeeCord 和 Velocity 三大主流服务器平台，让不同验证体系的玩家能够在同一服务器畅玩。

### 核心技术组件
- **编程语言**：Java（主） + Kotlin（辅）
- **服务器框架**：Bukkit/BungeeCord/Velocity 三端支持
- **验证系统**：Yggdrasil 协议兼容
- **构建工具**：Gradle 依赖管理

👉 [【点击查看】2025年最新 Multilogin 优惠码及特价套餐活动方案汇总](https://bit.ly/multIlogin)

## 二、安装前准备事项

### 系统要求清单
1. **Java 环境**：必须安装 JDK 17+
2. **服务器类型**：已部署的 Bukkit/BungeeCord/Velocity 服务器
3. **插件文件**：最新版 MultiLogin.jar（建议从官方渠道获取）

## 三、详细安装配置流程

### 步骤1：获取插件文件
- 访问项目 GitHub Releases 页面
- 下载适配当前服务器版本的最新 JAR 文件

### 步骤2：插件部署
bash
# Bukkit/BungeeCord 服务器：
将 MultiLogin.jar 放入 /plugins/ 目录

# Velocity 服务器特殊配置：
1. 放入 /plugins/ 目录
2. 编辑 velocity.toml 启用插件

### 步骤3：首次运行配置
1. 启动服务器观察控制台加载日志
2. 自动生成的配置文件路径：
   
   /plugins/MultiLogin/config.yml
   
3. 关键配置项说明：
   - `auth-servers`: 外置登录服务器地址
   - `proxy-settings`: 代理连接参数
   - `compatibility-mode`: 多版本兼容开关

### 步骤4：功能验证
1. 使用不同验证方式的客户端测试登录
2. 检查玩家数据同步状态
3. 监控控制台错误日志

## 四、常见问题解决方案

**Q1**：插件加载失败怎么办？
- 检查 Java 版本是否符合要求
- 确认服务器核心兼容性

**Q2**：玩家无法跨验证登录？
- 检查 config.yml 中的服务器白名单设置
- 验证网络端口是否开放

**Q3**：如何升级插件版本？
1. 备份现有配置
2. 替换新版 JAR 文件
3. 对比新旧配置文件差异

通过本教程的详细指导，您已成功实现 Minecraft 服务器的多验证系统集成。如需获取更多高级功能配置技巧，建议定期查阅项目文档更新。