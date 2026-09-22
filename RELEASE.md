# 上架 SkillHub 填写表

按本表在 skillhub.cn 的发布页填写。填完上传本目录的 `SKILL.md`、`README.md` 及 `references/` 文件夹。

## 元数据

| 字段 | 填写值 |
|---|---|
| slug（唯一标识） | project-handoff |
| 名称（name） | 项目交接 |
| 英文名（displayName en） | Project Handoff |
| 版本 | 1.0.2 |
| 分类（category） | Developer Tools（开发者工具） |
| 支持平台 | WorkBuddy、Claude Code、Cursor、OpenClaw |

## 标签（tags）

项目交接、agent 交接、上下文转移、跨工具、handoff、onboarding、项目记忆、接手

## 描述（description_zh，中文，用于语义搜索）

当一个 agent 在某个项目上工作很久、要把项目转交给另一个 agent（可能是不同工具，如从 WorkBuddy 换到 Claude Code、Cursor、Cline）时使用。生成结构化的项目交接包（分层：入口卡、状态、决策与禁忌、能力、索引），让下一个 agent 快速接手、尽量还原上一个 agent 的能力；接手方也能快速读懂项目和用户需求。特点：省 token（分层按需加载、索引不搬原文、skill 自身轻量）、速度快（首次全量生成、之后增量维护活档案）、信息完整（未完成任务带目的/背景/现状/下一步/验收/优先级并挂靠项目目标，含给新 agent 的接手指令）。触发：交接项目、准备交接、生成交接包、把项目交给下一个 agent、handoff、接手项目、继续这个项目、快速上手这个项目、onboard。

## 描述（description_en，英文，用于语义搜索）

Use when an agent has worked on a project for a long time and needs to hand it off to another agent (possibly a different tool such as Claude Code, Cursor, or Cline). Generates a structured handoff pack (entry card, status, decisions, capabilities, index) so the next agent can onboard quickly and recover the previous agent's capabilities. Key features: token-efficient (layered on-demand loading, index instead of copying files), fast (full generation once, then incremental updates), and complete (unfinished tasks carry purpose, background, status, next-step, acceptance, and priority, linked to project goals). Triggers: handoff, project handoff, context transfer, onboard, switch agent, continue this project.

## 搜索可见性要点（为什么这么填）

- 语义搜索匹配的是 name、description、description_zh、tags。上面描述已覆盖用户最可能搜的词：交接、上下文转移、跨工具、handoff、onboard、接手、agent 切换、项目记忆等。
- 不要把描述写得太抽象（如"智能协作助手"），要落到具体动作和场景词上，才容易被 find-skills 搜到。

## 发布步骤

1. 登录 skillhub.cn，进入「发布 Skill」页。
2. 按上表填写，上传 `SKILL.md` + `README.md` + `references/`。
3. 提交审核（三线安全审核：内容合规 + 漏洞扫描 + AI 安全评估）。
4. 审核通过后自动上架，用户即可用 find-skills 搜索到。
