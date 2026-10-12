# my-skills

我自己做的 AI skill 合集。skill 就是一份写给 AI 的“说明书”，装上以后，AI 遇到对应的问题就会按说明书的方式来回答。

## 目前有的 skill

| skill | 干什么 |
|---|---|
| [science-explainer（科普知识讲解员）](science-explainer/SKILL.md) | 什么知识都能问。先联网查百科、教科书、权威机构报告，再用大白话和生活比喻讲明白；每条说法都标出处，权威来源说法不一致时分别列出、不评对错。 |

## 怎么安装

### 方法一：一条命令装好（适用于 Claude Code、Codex、Cursor 等几十种 AI 编程工具）

电脑上需要先装好 [Node.js](https://nodejs.org/)，然后运行：

```bash
npx skills add 2763945400-ctrl/my-skills
```

只装其中一个 skill：

```bash
npx skills add 2763945400-ctrl/my-skills --skill science-explainer
```

### 方法二：手动复制（Claude Code）

把 `science-explainer` 整个文件夹复制到：
- Windows：`C:\Users\你的用户名\.claude\skills\`
- Mac / Linux：`~/.claude/skills/`

### 方法三：Claude 网页版 / 桌面版

把 `science-explainer` 文件夹压缩成 zip，在 Claude 的设置里找到 Skills（技能）页面上传。

### 其他不支持 skill 的 AI

打开 [science-explainer/SKILL.md](science-explainer/SKILL.md)，把 `---` 下面的正文复制下来，粘贴到对话开头或 AI 的“自定义指令”里。效果会差一些。

## 用起来是什么样

装好后直接问就行，比如“为什么会有四季？”“科普一下潜艇怎么下潜”。回答大概长这样（节选）：

> **一句话答案**
> 因为地球是“歪着”绕太阳转的，不是因为离太阳时远时近。
>
> **权威说法**
> 地球自转轴相对公转平面倾斜约 23 度……——NASA Science「Seasons on Earth, Mars and Beyond」
>
> **大白话**
> 地球的“轴”是斜着的，而且一年到头斜的方向不变……
>
> **常见误解**
> “夏天热是因为离太阳近。”不对：南北半球季节相反，如果是距离造成的，全球应该同时过夏天。
>
> **查询记录**
> 搜索工具：WebSearch｜关键词：why do we have seasons axial tilt NASA｜日期：2026-10-12

## 注意

- 这个 skill 需要 AI 能上网搜索。不能上网时，它会在开头说明“未经核实，仅供参考”。
- 它只做知识科普：武器、毒物等话题只讲原理和历史；医疗、法律、投资类内容不能替代专业意见。
