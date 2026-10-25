# DSHAgentMD

DSH（DeepSeek Harness）使用的 Agent MD —— 全局规则文件的版本备份。

## 内容

- `AGENTS.md`：`~/.dsh/AGENTS.md` 的原样副本，是 DSH 在所有工作区都遵守的全局规则（工作区初始化、读取/提交规则、经验文档规范、环境说明）。

## 为什么单独存一份

`~/.dsh/AGENTS.md` 在本机，换电脑或重装就没了。推到 GitHub 后可以随时取回，也能看历史改动。

## 同步方式

改动全局规则后，在本目录执行：

```sh
cp ~/.dsh/AGENTS.md ./AGENTS.md
git add AGENTS.md
git commit -m "同步全局 Agent MD"
git push
```

## 注意

- 这里是**个人**规则文件，不含密码、Key、客户隐私；新增规则时也保持这一点。
- `不推送/` 是本地草稿目录，已被全局 ignore 挡住，不会进仓库。
