# Agent Handoff Kit

把一项任务交给另一个 AI 时，带上目标、最新纠正、已有成果和接得住的下一步。

这是给研究、写作和创作任务使用的文字工具包。下载文件，把模板填好并交给接手的 AI，就可以开始一次交接。首版没有服务端、模型 API、自动触发或跨账号连接。

## 从一个示例开始

1. 打开[写作任务示例](examples/01-writing/START_HERE.md)，把其中的任务包交给另一个 AI。
2. 用[接收方提示词](prompts/receive-handoff.md)开始。
3. 收到结果后，对照[检查参考](examples/01-writing/review.md)，判断它是否落实最新纠正。
4. 换成自己的任务时，复制[交接卡](templates/handoff.md)。

还可以阅读[材料不完整的示例](examples/02-missing-evidence/START_HERE.md)，看怎样交回已完成的部分并留下具体断点。

## 交接卡里保留什么

| 信息 | 它帮助接手者回答什么 |
| --- | --- |
| 目标与本次范围 | 最后要做成什么，这一轮推进哪部分 |
| 已有成果与依据 | 已经有什么，实际材料在哪里 |
| 现行决定与最新纠正 | 现在沿用什么，哪条旧说法已经被替代 |
| 下一步与检查标准 | 接下来能做什么，怎样判断做对了 |
| 停点与责任 | 缺少什么，谁能处理，哪些部分仍可继续 |
| 回程与后续 | 结果交到哪里，由谁检查，检查后怎样接上 |

交接者留下可读取的材料，接手者实际读取并完成动作，接收方检查结果。三步分别记录。

## 文件导航

- [快速开始](docs/quickstart.md)
- [交接卡](templates/handoff.md)
- [决定与纠正记录](templates/decisions.md)
- [成果交回卡](templates/return.md)
- [结果检查表](templates/review.md)
- [接收方提示词](prompts/receive-handoff.md)
- [示例一：修改文案并保留约定范围](examples/01-writing/START_HERE.md)
- [示例二：缺少音频时怎样保留断点](examples/02-missing-evidence/START_HERE.md)
- [能力范围与检查记录](docs/scope-and-validation.md)
- [反馈与维护](CONTRIBUTING.md)

## 先填最少的信息

一个小任务，可以先写清楚：目标、材料、最新决定、下一步、完成标准、交回位置。只有当旧结论、多人分工或材料版本影响判断时，再展开相应字段。未知项写明未知。

```text
目标：
材料：直接粘贴正文，或附上接手者能打开的文件。
最新决定：现在按什么做，替代了哪条旧要求。
下一步：这一轮完成哪一个具体动作。
完成标准：结果里必须有什么，哪些内容需要保留。
交回位置：结果放在哪里，由谁检查。
```

## 适合谁

正在用多个 AI 做真实项目，希望减少重复解释、保留纠正，并在收到结果后继续推进的个人或小团队。

模板适合人工复制或文件交接。自动读取、自动执行、消息发送和持续回写，需要另行接入与验证。这些文件不会自动获得其他工具的访问权或执行授权。

## 首版状态

v0.1.0 候选版。已有两个自包含演示、模板与场景走查；未经过外部用户或独立模型试用。示例为专门编写的虚构材料，不是客户记录，也不是对任何工具效果的基准测试。检查详情见[范围说明](docs/scope-and-validation.md)。

## English summary

A text-first handoff kit for research, writing, and creative work across AI assistants.

Keep the goal, accessible artifacts, current decisions, superseded instructions, next action, acceptance criteria, and return destination together. The receiver reads the actual materials and produces a concrete result. A reviewer then checks it and records the next step.

Start with the self-contained [writing example](examples/01-writing/START_HERE.md), then copy the [handoff template](templates/handoff.md) for your own task. The [missing-evidence example](examples/02-missing-evidence/START_HERE.md) shows how to deliver a useful partial result without inventing unavailable evidence.

This release is a manual document kit. It is not an autonomous memory service and does not connect accounts. The examples are fictional fixtures; external user testing and independent model evaluation have not been completed.

## License

[MIT](LICENSE). 保留许可与版权声明即可按许可使用、修改和分发。本仓库不包含私人项目资料、聊天原文或服务配置。

## 维护与反馈

由 Arden 整理与维护。使用问题可通过仓库 Issues 反馈，建议提供一个能复现问题的自拟示例。公开反馈前请删除姓名、私人邮箱、密钥和私人资料链接，具体方式见[反馈说明](CONTRIBUTING.md)。
