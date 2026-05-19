# Codex Imagegen Skill

[中文](README.md)

Personal backup and customization repo for the Codex `imagegen` skill.

This repository tracks local changes so updates from the system-installed skill can be reviewed with Git before custom edits are lost.

## Files

- `SKILL.md` - main skill instructions
- `references/` - prompt and API references
- `scripts/` - helper scripts for image generation and post-processing
- `assets/` - skill assets
- `config.example.json` - example config file

## Local Config

Real local config must stay untracked:

```text
config.json
```

Create it from the example if needed:

```powershell
Copy-Item config.example.json config.json
```

Then edit `config.json` locally. Do not commit API keys.

## Common Commands

Check local changes:

```powershell
git status
git diff
```

Commit custom changes:

```powershell
git add .
git commit -m "update imagegen skill"
git push
```

After the system updates this skill, review what changed:

```powershell
git status
git diff
```
