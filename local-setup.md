# 本地 Git 连接 GitHub 说明

本文件由 WorkBuddy 自动生成，用于验证并记录本机与 GitHub 的连接配置。

## 配置方式

| 项目 | 值 |
| --- | --- |
| 传输协议 | HTTPS |
| 凭据存储 | Windows 凭据管理器（Git Credential Manager） |
| 提交身份 | hasbite / 3659419436@qq.com |
| 默认分支 | main |

Token 未以明文形式写入任何项目文件，保存在系统凭据管理器中，由 Git 自动调用。

## 常用命令

```bash
# 查看远端状态
git ls-remote origin

# 拉取最新代码
git pull

# 提交并推送
git add .
git commit -m "说明性提交信息"
git push

# 新建并推送分支
git checkout -b feature/xxx
git push -u origin feature/xxx
```

## 注意

- Token 具有 `repo` 范围，即所有仓库的读写权限，有效期 30 天。
- 到期后需在 GitHub 重新生成 Token，并通过 `git credential approve` 更新凭据管理器中的记录。
