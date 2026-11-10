# git-practice

一个用来练手的小仓库，用来确认 Git 环境（Git + VS Code + GitHub）已经配置正确。

## 这个仓库里有什么

| 文件 | 说明 |
|---|---|
| `README.md` | 就是这份说明 |
| `hello.py` | 一个最小的 Python 脚本 |
| `.gitignore` | 常见的忽略规则（编辑器、Python、Node、Windows 临时文件） |

## 常用命令速查

```bash
git status                # 看当前有哪些改动
git add .                 # 把改动放入暂存区
git commit -m "说明"       # 提交
git log --oneline         # 看提交历史
git remote -v             # 看远程仓库地址
git push                  # 推送到 GitHub
git pull                  # 拉取远程更新
```

## 小提示

- 提交信息写「做了什么」，例如 `修复登录页按钮错位`，不要写 `update`。
- 提交前先 `git status` 确认改动的文件，避免把无关文件带上。
- 分叉时 `git pull` 会报 `Not possible to fast-forward`（这是本机配置的“仅快进”策略），此时用 `git pull --rebase` 或 `git pull --no-rebase`。
