# AI 家庭顾问（AI Family Counselor）

面向青少年心理健康与家庭沟通场景的 AI 辅助沟通产品。项目以家庭为基本单元，通过多成员对话、角色识别和家庭沟通分析报告，帮助家庭更有结构地开展沟通与家庭会议。

> 本项目用于研究与辅助沟通，不替代心理治疗、医疗诊断或紧急危机干预。若存在自伤、自杀、暴力等紧急风险，请立即联系当地紧急服务、学校心理老师或专业医疗机构。

## 项目背景

青少年心理健康问题日益受到关注，而家庭沟通往往是影响青少年情绪支持、亲子关系与心理复原力的重要因素。本项目通过访谈、文献研究、市场问卷和竞品分析，聚焦“如何让更多家庭获得可负担、可持续的沟通支持”。

研究团队访谈了学生、家长、教师、家庭顾问及 AI 技术从业者，并结合家庭顾问组织家庭会议的实践经验，形成了“AI 家庭顾问”的产品思路：以不评判、可追溯、可行动的方式帮助家庭理解沟通模式，并促成平等、尊重的家庭对话。

## 核心能力

- 多成员家庭对话与角色识别
- 聊天模型与报告模型的独立配置
- 家庭沟通分析报告生成
- 后台可视化模型管理：新增、编辑、删除模型；设置聊天模型或报告模型；API Key 脱敏展示
- 支持家庭会议的议题梳理与沟通建议
- 通过数据脱敏与加密机制保护敏感信息

## 研究摘要

本研究围绕“AI 家庭顾问”探索人工智能支持家庭沟通、进而促进青少年心理健康的可行路径。产品具备多成员沟通、角色识别、家庭沟通分析报告生成及家庭会议支持等能力。

研究在 25 个试用家庭中开展前后测，使用青少年亲子沟通量表（PACS）和青少年心理韧性量表（RSCA）评估变化。试用结果显示，产品与家庭沟通质量提升、青少年复原力改善及家庭对家庭会议接受度提高存在积极关联；但受样本规模等限制，结论仍需在更大样本与更长期研究中进一步验证。

**关键词：** 青少年心理健康、AI 家庭顾问、青少年复原力、家庭沟通质量、家庭会议

## Abstract

AI Family Counselor is an AI-assisted family communication solution designed in response to adolescent mental-health needs and gaps in accessible family support. It supports multi-member conversations, role recognition, family communication analysis reports, and family meetings.

The research combined interviews, literature review, market surveys, and competitor analysis. A pilot involving 25 families used the Parent-Adolescent Communication Scale (PACS) and the Resilience Scale for Chinese Adolescents (RSCA). The findings suggest positive associations with family communication quality, adolescent resilience, and acceptance of family meetings. Given the limited sample size, further validation with larger and longer-term studies is needed.

**Keywords:** Adolescent mental health, AI Family Counselor, adolescent resilience, family communication quality, family meeting

## 项目结构

```text
AI家庭顾问/
├── AIFamilyConsultant_NewBackend_runable/   # Spring Boot 后端
├── AIFamilyConsultant_NewFrontend_User/     # 聊天前端
├── AIFamilyConsultant_NewFrontend_Admin/    # 后台管理前端
└── README.md
```

## 本次版本更新（v1.1.0）

本次更新重点为“模型管理可视化”：

- 新增后台模型管理页面
- 可分别指定聊天模型与报告模型
- 支持通过后台维护模型名称、模型 ID 与 API Key
- API Key 仅展示脱敏信息，编辑时留空可保留原值
- 聊天与报告统一使用后台已配置的模型

## 技术说明

- 后端：Java / Spring Boot
- 聊天前端：React / Vite
- 后台管理前端：React / Umi Max
- 数据库：MySQL
- 缓存：Redis
- 大语言模型：通过后台模型管理配置并调用

## 版本

- `v1.0.0`：首次发布的基础版本
- `v1.1.0`：新增可视化模型管理，并支持分别配置聊天模型与报告模型
