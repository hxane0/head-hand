# GitHub同步指南

仓库：https://github.com/hxane0/head-hand

## 日常同步

在笔记文件夹打开终端。开始前：

```powershell
git status
git pull --ff-only
```

写完先检查改动，然后上传：

```powershell
git diff
git add -- "具体目录/具体笔记.md"
git diff --cached
git commit -m "补充学习笔记"
git push
```

新文件需直接打开检查。确认所有改动都需要上传时可以使用git add .。

## 另一台电脑

在空的目标位置运行：

```powershell
git clone https://github.com/hxane0/head-hand.git
cd head-hand
```

每次开始前拉取，结束后提交并推送。

## 问题处理

认证失败时检查账号与权限。历史分叉时先检查双方提交，再明确合并或变基并解决冲突，不强制推送掩盖问题。不要上传密钥、敏感信息和未经许可的资料。大型数据与模型先确定存储方式。Obsidian本地配置已排除。
