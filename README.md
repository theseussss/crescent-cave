# 斜月三星洞

> 斜月三星，写出来是个"心"字。
> 从来就没有斜月三星洞——你要找的东西，本来就在你自己心里。

一个 Claude Code skill，通过多视角并行分析，为你的人生困惑、哲学反思和个人成长提供来自不同思想传统的回应。

## 它做什么

当你提出一个关于人生、内心体验或价值选择的问题时，斜月三星洞会：

1. 从视角库中自动选择 3-5 个最相关的视角
2. 为每个视角启动一个独立的子 agent 进行深度分析
3. 综合呈现各视角的**共振**与**分歧**
4. 支持多轮对话——视角会根据你的新体验修正自己的判断

像几个不同传统的师傅在认真对待你的问题。

## 视角库（17 个，持续增加）

**中国传统：** 道家 · 儒家 · 佛教 · 墨家 · 法家 · 兵家

**西方学术：** 深度心理学（荣格/温尼科特/IFS） · 现象学（梅洛-庞蒂/海德格尔） · 斯多葛 · 维特根斯坦 · 齐泽克

**全球南方：** Ubuntu · 苏非 · 吠檀多

**虚拟角色：** 润州刘炼（永劫无间）

## 安装

1. 将 `SKILL.md` 和 `perspectives/` 目录复制到 `~/.claude/skills/crescent-cave/`
2. 重启 Claude Code
3. 使用 `/crescent-cave` 调用

```bash
# 快速安装
mkdir -p ~/.claude/skills/crescent-cave
cp SKILL.md ~/.claude/skills/crescent-cave/
cp -r perspectives ~/.claude/skills/crescent-cave/
```

## 添加新视角

1. 在 `perspectives/` 下创建 `{id}.md`，按模板填写角色档案
2. 在 `perspectives/_index.md` 中添加一行索引
3. 同步到 `~/.claude/skills/crescent-cave/perspectives/`

角色档案模板见 [SKILL.md](SKILL.md) 中的"视角库管理"部分。

## 起源

这个项目诞生于一次关于"元婴"的对话。从"什么是元婴"出发，经过对内在小孩、身体修炼、入世修行的探讨，最终发现：多个视角同时照亮同一个体验时，能看到单一视角看不到的东西。于是把这个对话模式做成了工具。

> 精金百炼，方可至臻。——润州刘炼

## License

MIT
