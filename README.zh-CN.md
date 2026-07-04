# Paper Mentor Skill 中文说明

把模糊的论文问题，变成像导师组会议一样清楚的 AI 讨论。

`paper-mentor` 是一个 Codex skill，面向学生和研究者，覆盖选题、摘要、Introduction、Related Work、实验设计、投稿前预审、审稿意见回复，以及如何更好地向 AI 提问。

它的重点不是代写论文，而是帮学生更会思考、更会提问、更早发现风险。

## 最推荐的试用方式

安装后，在新对话里复制：

```text
Use $paper-mentor in Paper Health Check mode.

研究方向：
目标会议 / 期刊 / 读者：
材料类型：选题 / 摘要 / Introduction / 完整草稿
我的核心贡献：
我最担心的问题：

正文：
[粘贴你的内容]
```

它会输出：

- 一句话诊断
- 风险评分
- 阻塞问题
- 修改优先级
- 下一步三件事
- 接下来更适合问 AI 的 prompt

## 八个模式

| 模式 | 用途 |
| --- | --- |
| Prompt Clinic | 把模糊问题改成高质量 AI prompt |
| Paper Health Check | 快速体检选题、摘要、引言或草稿 |
| Contribution Mapper | 梳理 gap、创新点、证据和贡献表达 |
| Section Surgeon | 修改摘要、Introduction、Related Work、Method 等章节 |
| Literature Map | 把文献列表组织成 Related Work 结构 |
| Methods Audit | 检查实验、baseline、metric、ablation 是否支撑结论 |
| Reviewer Simulation | 模拟投稿前审稿，找最可能被拒的原因 |
| Rebuttal Planner | 分析审稿意见，规划回复和正文修改 |

## 临时试用

这个 skill 默认是手动调用：

```yaml
policy:
  allow_implicit_invocation: false
```

也就是说，只有你明确写 `$paper-mentor` 时才会使用它。

Windows 临时安装：

```powershell
git clone https://github.com/YuzeLumos/paper-mentor-skill.git
New-Item -ItemType Directory -Force "$env:USERPROFILE\.codex\skills"
Copy-Item -Recurse -Force ".\paper-mentor-skill\paper-mentor" "$env:USERPROFILE\.codex\skills\"
```

试完删除：

```powershell
Remove-Item -Recurse -Force "$env:USERPROFILE\.codex\skills\paper-mentor"
```

## 可复制 Prompt

更多模板见 [PROMPTS.md](PROMPTS.md)。

最常用的一个：

```text
Use $paper-mentor in Reviewer Simulation mode.

研究方向：
目标会议 / 期刊 / 读者：
核心贡献：
已有证据：

摘要和 Introduction：
[粘贴内容]

请用 Advisor、Reviewer 2、Method Auditor、Writing Coach 的方式评审，最后给出拒稿风险和下一步三件事。
```
