# GitHub-Release - Claude Code Skills

Claude Code Skills 发布仓库，用于存储和管理 Claude Code 的自定义技能。

## 功能介绍

本仓库包含以下 Claude Code Skills：

- 📦 **publish-to-github** - GitHub 发布助手
  - 帮助用户将项目发布到 GitHub
  - 支持初始化 git、添加文件、创建提交、配置远程仓库和推送代码
  - 自动提醒创建详细的 README 文件

## 安装步骤

### 1. 克隆仓库

```bash
git clone git@github.com:quzp1993/GitHub-Release.git
cd GitHub-Release
```

### 2. 复制 skill 文件

将 `skills/` 目录下的 `.md` 文件复制到您的 Claude Code skills 目录：

**Windows**:
```
C:\Users\YourName\.claude\skills\
```

**macOS/Linux**:
```
~/.claude/skills/
```

例如：
```bash
cp skills/publish-to-github.md ~/.claude/skills/
```

### 3. 重启 Claude Code

重启 Claude Code 使 skills 生效。

## 使用方法

### publish-to-github

在 Claude Code 对话中使用：

```
帮我发布到 GitHub
```

skill 会引导您完成以下步骤：
1. 检查 Git 仓库状态
2. 配置 Git 用户信息（如需要）
3. 添加文件到暂存区
4. 创建/更新 README 文件
5. 创建提交
6. 设置远程仓库
7. 推送代码到 GitHub

**指定目标仓库**：
```
帮我发布到 git@github.com:quzp1993/your-repo.git
```

## 功能说明

### publish-to-github

完整的 GitHub 发布工作流程，包括：

- ✅ 检查和初始化 Git 仓库
- ✅ 配置 Git 用户信息
- ✅ 添加文件到暂存区
- ✅ 自动提醒创建 README 文件
- ✅ 创建格式化的提交信息
- ✅ 设置远程仓库（HTTPS/SSH）
- ✅ 推送代码到 GitHub
- ✅ 处理常见问题（冲突、认证失败等）

## 文件说明

| 文件 | 说明 |
|------|------|
| `skills/publish-to-github.md` | GitHub 发布助手 skill |
| `README.md` | 本项目说明文档 |
| `LICENSE` | MIT 许可证 |

## 常见问题

### Q: 如何添加新的 skill？

A: 将新的 `.md` skill 文件放入 `skills/` 目录，提交并推送到 GitHub。

### Q: skill 不生效怎么办？

A: 确认 skill 文件在正确的目录，并重启 Claude Code。

### Q: 如何配置 GitHub SSH 密钥？

A: 参考 skill 文件中的"权限被拒绝（SSH方式）"章节。

## 安全注意事项

- 提交前检查文件内容，避免泄露敏感信息
- 使用 `.gitignore` 排除敏感文件
- SSH 方式比 HTTPS 方式更安全且便捷

## 许可证

本项目采用 MIT 许可证 - 详见 [LICENSE](LICENSE) 文件

## 贡献

欢迎提交 Issue 和 Pull Request！

## 相关链接

- [Claude Code 官方文档](https://docs.anthropic.com)
- [GitHub 官方文档](https://docs.github.com)
