# PMP & ITIL Delivery SOP

把 PMP 的项目治理和 ITIL 4 的服务运营连接起来的一套轻量 SOP、模板与 Agent Skill。

它适合客户项目、系统建设、上线交接、服务运营、需求变更、故障处理和持续改进。目标不是增加流程负担，而是让每个阶段都有清晰的结果、责任、决策、沟通与记录。

## 适合谁

- 项目经理、交付经理、客户成功/服务经理
- 需要同时管理项目交付与上线后服务的团队
- 希望让 AI Agent 与人工团队遵循同一套工作方式的组织

## 仓库结构

```text
.
├── README.md                         # 人类读者的入口
├── AGENTS.md                         # AI Agent 的仓库级工作说明
├── docs/
│   └── lifecycle-sop.md              # 人类可读的全生命周期 SOP
├── templates/                        # 可直接复制填写的工作模板
│   ├── project-intake.md
│   ├── weekly-service-review.md
│   ├── change-assessment.md
│   ├── incident-problem-record.md
│   └── service-handover.md
└── skills/
    └── pmp-itil-delivery-sop/        # Agent 可加载的 Skill
        ├── SKILL.md
        └── references/lifecycle-sop.md
```

## 使用方式

### 人工团队

1. 新项目或客户需求进入时，先使用 `templates/project-intake.md`。
2. 在交付期，用 `templates/weekly-service-review.md` 固定同步进展、风险、问题和待决策事项。
3. 出现服务故障、反复问题或需求变化时，使用相应模板并遵循 `docs/lifecycle-sop.md` 的路由规则。
4. 上线前使用服务交接清单，避免“项目交付了但没人能稳定运营”。

### AI Agent

Agent 应先阅读根目录的 `AGENTS.md`，再读取 `skills/pmp-itil-delivery-sop/SKILL.md`。当任务需要全生命周期规划、变更、事件、服务交接或客户管理时，继续读取 Skill 所链接的参考文件。

若使用 Codex，可将 `skills/pmp-itil-delivery-sop/` 复制到个人的 Codex skills 目录后，通过 `$pmp-itil-delivery-sop` 调用。

## 快速决策

| 情况 | 首选处理方式 |
|---|---|
| 新客户诉求或新项目 | 先澄清价值、范围、约束、决策人和风险 |
| 标准化、重复性需求 | 作为服务请求，通过目录交付 |
| 服务中断或质量下降 | 先恢复服务并沟通，随后再复盘 |
| 反复或重大故障 | 建立问题记录，分析根因、已知错误和永久修复 |
| 未承诺的敏捷需求/缺陷 | 进入 Backlog，由 PO 排序 |
| 影响承诺、基准或服务配置的改动 | 做影响评估，按变更流程取得授权 |
| 上线交付 | 确认支持、监控、知识、回滚和责任已具备 |

## 核心原则

- 聚焦客户和业务价值，不只关注任务完成。
- 先澄清、评估和沟通，再承诺、升级或改变计划。
- 把未来不确定性记为风险；把当前中断记为问题或事件。
- 事件先恢复；问题再找根因；变更必须受控。
- 项目结束不等于工作结束；完成服务交接和运营就绪才算真正闭环。

## 发布前建议

本仓库未预设许可证。公开发布前，请根据你的使用方式补充 LICENSE、贡献指南和组织定制说明。
