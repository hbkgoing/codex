# Codex

Codex 是一个用于记录与演示的示例仓库，后续将逐步补充功能代码与文档。

## 目录

- [背景](#背景)
- [功能规划](#功能规划)
- [快速开始](#快速开始)
- [贡献](#贡献)
- [许可](#许可)

## 背景

该仓库用于沉淀实验、规范化模板以及项目演示材料。

## 功能规划

- 初始化项目结构与基础文档
- 添加示例代码与使用说明
- 补充测试与持续集成配置

## 快速开始

### 前置条件

- Java 17
- Maven 3.9+

### 本地运行

```bash
mvn spring-boot:run
```

### 访问 Hello World

启动后访问：

```bash
curl http://localhost:8080/
```

预期返回：

```text
Hello, World!
```

### 运行测试

```bash
mvn test
```

## CI/CD

仓库包含 GitHub Actions 流水线，可在推送到 `main` 分支时构建并通过 SCP 上传构建产物。请先在仓库 Secrets 中配置：

- `DEPLOY_HOST`：服务器地址
- `DEPLOY_PORT`：SSH 端口（例如 22）
- `DEPLOY_USER`：登录用户名
- `DEPLOY_SSH_KEY`：SSH 私钥内容（建议使用专用部署密钥）
- `DEPLOY_TARGET_DIR`：服务器上的目标目录（例如 `/home/hbk/app`）

## 贡献

欢迎提交 Issue 与 Pull Request。请在提交前确保描述清晰，并附上必要的测试或复现步骤。

## 许可

待定。
