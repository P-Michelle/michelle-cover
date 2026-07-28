# AI 知识博主封面 Skill

一套把「真人照片 → 高点击率封面」标准化的 Agent Skill。风格是 **YouTube Thumbnail × 小红书爆款知识博主封面** 的融合：真人 IP 放右侧、超大标题占左侧、奶油黄重点词、白字黑描边、自然办公背景、不过度美颜。

核心不是设计感，是**点击率**——在小红书两列信息流的缩略图尺寸下，用户 1 秒内要能看清标题、认出人物、判断主题。

## 效果示例

以下封面均由本 Skill 的公式生成——真人 IP（右侧）＋ 超大标题（左侧）＋ 奶油黄重点词 ＋ 橙色数字 ＋ 自然背景：

<table>
  <tr>
    <td width="25%"><img src="assets/cover-01.jpg" alt="文科生转行AI，这个岗位有壁垒"></td>
    <td width="25%"><img src="assets/cover-02.jpg" alt="To B 领域，文科生转行 AI 岗位天花板"></td>
    <td width="25%"><img src="assets/cover-03.jpg" alt="24 小时内找到真正适合你的 AI 转行赛道"></td>
    <td width="25%"><img src="assets/cover-04.jpg" alt="AI 是文科生最大的时代红利"></td>
  </tr>
</table>

## 安装

这是标准 Agent Skill，把 `michelle-cover` 目录放到对应位置即可：

- **Claude Code**：复制到 `~/.claude/skills/michelle-cover`
- **Codex**：复制到 `~/.codex/skills/michelle-cover`
- **通用 Agent（豆包 / Trae 等）**：复制到 `~/.agents/skills/michelle-cover`

```bash
git clone https://github.com/P-Michelle/michelle-cover.git
cp -r michelle-cover ~/.claude/skills/
```

## 使用

1. 准备一张你的**人像照片**（真人 IP，用于做图生图）。
2. 想好**标题文字**（2–4 行，含 1 个重点词 + 1 个数字）。
3. 对 Agent 说：「用 michelle-cover 帮我做张封面，标题是 XXX」，并附上人像照片。
4. Agent 会套用主提示词 + 你的照片做图生图，出图后按自检清单校验。

标题示例：

```
24 小时内 / 找到真正适合你的 / AI 转行赛道
文科生 / 零基础转行 AI / 唯一正确的思路
```

## 文件说明

- [`SKILL.md`](SKILL.md) — 技能主体：流程、主提示词、排版骨架、出图自检清单
- [`references/style-guide.md`](references/style-guide.md) — 完整分模块风格规范
- `assets/` — 放你的封面示例图

## 一起共建

用的过程中有问题、有更好的提示词或案例，欢迎提 Issue / PR，一起把这套封面公式打磨得更好。

## License

MIT
