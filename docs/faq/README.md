# 雷泽 FAQ · 团队知识库

把客户 RFQ 中的共性问题变成可追溯、可审核的中英文答案。

**官网原文迁移及样例修订均通过 PR 审核。** 样例 PR 的新增与修订答案均为草稿；现有官网没有被修改。本次没有开启定时采集、自动发布或 Nextcloud 同步。

| 我想做什么 | 从这里开始 |
|---|---|
| 阅读官网原有中文 FAQ | [中文原文目录](website-original/zh-CN/README.md) |
| Read existing English FAQ | [English originals](website-original/en/README.md) |
| 看新增中文草稿 | [中文目录](https://github.com/ReZ-TI/faq/blob/codex/faq-content-sample-20261105/docs/faq/zh-CN/README.md) |
| 看新增英文草稿 | [English index](https://github.com/ReZ-TI/faq/blob/codex/faq-content-sample-20261105/docs/faq/en/README.md) |
| 提一个修改建议 | [查看示例修改建议 #1](https://github.com/ReZ-TI/faq/issues/1) |
| 学会提交与审核 | [团队操作说明](CONTRIBUTING.md) |
| 看现有官网原文与待核验问题 | [来源说明](sources/README.md) |
| 看上线条件与权限现状 | [维护与发布](GOVERNANCE.md) |

## RFQ → FAQ

客户 RFQ → 提炼共性问题 → Issue 收集建议和依据 → PR 对比修改 → Kelvin 审核 → 合并正式版本 → 按公开范围发布。

客户文件保存在 Odoo / Nextcloud，FAQ 引用有权限控制的来源。通用答案中去除客户姓名、联系方式、议价金额与项目细节。

## 这套样板里有什么

- 官网现有 10 组中英文 FAQ 的[可读原文](website-original/README.md)及来源快照，用于对照；迁移不等于全部说法已重新核实。
- 6 组中英文问答草稿，涵盖控制选项、询价、风扇灯、海外需求和兼容性边界。
- 一张“FAQ 修改建议”表单和一份 PR 模板。
- 一条明确标注为模拟的 RFQ 示例，展示从问题到答案的过程。
- 稳定编号、依据、适用范围、核验日期、审核状态和中英文对应关系。

## 提交修改

不会操作 PR 的同事：现在就在 **Issues → New issue → FAQ 修改建议** 填表即可。

会操作 PR 的同事：按[团队操作说明](CONTRIBUTING.md)编辑文件，在新分支提交 PR。

Issue 表单和默认 PR 模板已放入独立 FAQ 仓库的默认分支，可以使用。答案样例在 PR 中待审核。

## 先认识两个限制

1. 仓库公开可读。默认分支通过 PR 更新，由 Kelvin 负责内容审核；具体规则状态以 GitHub 仓库设置为准。
2. 本次连接使用 Kelvin 的 GitHub 账号。GitHub 不允许作者给自己的 PR 点 Approve；这次可查看差异、评论并决定是否合并。正式由同事或独立机器人账号提 PR，再由 Kelvin 审批。
