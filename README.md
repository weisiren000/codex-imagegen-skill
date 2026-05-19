# Codex Imagegen Skill

[English](README.en.md)

这是 Codex `imagegen` skill 的个人备份和魔改仓库。

这个仓库用于跟踪本地修改。以后系统自动更新或覆盖 skill 后，可以直接用 Git 查看变化，避免自己的改动丢失。

## 文件说明

- `SKILL.md` - skill 主说明文件
- `references/` - prompt、API 和使用参考
- `scripts/` - 图片生成和后处理辅助脚本
- `assets/` - skill 资源文件
- `config.example.json` - 配置示例文件

## 本地配置

真实配置文件必须保持不被 Git 跟踪：

```text
config.json
```

需要时可以从示例复制：

```powershell
Copy-Item config.example.json config.json
```

然后只在本地编辑 `config.json`。不要提交 API Key。

## 常用命令

查看本地变化：

```powershell
git status
git diff
```

提交自己的修改：

```powershell
git add .
git commit -m "更新 imagegen skill"
git push
```

系统更新或覆盖 skill 后，查看发生了什么变化：

```powershell
git status
git diff
```
