# AI 家庭顾问 / AI Family Counselor

面向青少年心理健康与家庭沟通场景的 AI 辅助沟通产品。项目以家庭为基本单元，通过多成员对话、角色识别和家庭沟通分析报告，帮助家庭更有结构地开展沟通与家庭会议。  
An AI-assisted communication product for adolescent mental-health and family-communication settings. Centered on the family unit, it supports multi-member conversations, role recognition, and family communication analysis reports to help families communicate and hold family meetings more constructively.

> 本项目用于研究与辅助沟通，不替代心理治疗、医疗诊断或紧急危机干预。若存在自伤、自杀、暴力等紧急风险，请立即联系当地紧急服务、学校心理老师或专业医疗机构。  
> This project is for research and communication support only. It does not replace psychotherapy, medical diagnosis, or emergency intervention. For immediate risks involving self-harm, suicide, or violence, contact local emergency services, a school counselor, or qualified medical professionals immediately.

## 项目背景 / Project Background

青少年心理健康问题日益受到关注，而家庭沟通往往是影响青少年情绪支持、亲子关系与心理复原力的重要因素。本项目通过访谈、文献研究、市场问卷和竞品分析，聚焦“如何让更多家庭获得可负担、可持续的沟通支持”。  
Adolescent mental health has become an increasingly important concern. Family communication is often a key factor in emotional support, parent-adolescent relationships, and resilience. Through interviews, literature review, market surveys, and competitor analysis, this project explores how to provide affordable and sustainable communication support for more families.

研究团队访谈了学生、家长、教师、家庭顾问及 AI 技术从业者，并结合家庭顾问组织家庭会议的实践经验，形成了“AI 家庭顾问”的产品思路：以不评判、可追溯、可行动的方式帮助家庭理解沟通模式，并促成平等、尊重的家庭对话。  
The team interviewed students, parents, teachers, family counselors, and AI practitioners. Drawing on family-counseling experience in facilitating family meetings, it developed the AI Family Counselor concept: helping families understand communication patterns in a nonjudgmental, traceable, and actionable way, while encouraging equitable and respectful dialogue.

## 核心能力 / Core Capabilities

- 多成员家庭对话与角色识别 / Multi-member family conversations and role recognition
- 聊天模型与报告模型的独立配置 / Independent configuration of chat and report models
- 家庭沟通分析报告生成 / Family communication analysis report generation
- 后台可视化模型管理：新增、编辑、删除模型；设置聊天模型或报告模型；API Key 脱敏展示 / Visual model management: create, edit, and delete models; assign chat or report models; display masked API keys
- 支持家庭会议的议题梳理与沟通建议 / Family-meeting topic organization and communication suggestions
- 通过数据脱敏与加密机制保护敏感信息 / Protection of sensitive information through data masking and encryption

## 研究摘要 / Research Abstract

本研究围绕“AI 家庭顾问”探索人工智能支持家庭沟通、进而促进青少年心理健康的可行路径。产品具备多成员沟通、角色识别、家庭沟通分析报告生成及家庭会议支持等能力。  
This research explores the feasibility of using AI Family Counselor to support family communication and, in turn, promote adolescent mental health. The product supports multi-member communication, role recognition, family communication analysis reports, and family meetings.

研究在 25 个试用家庭中开展前后测，使用青少年亲子沟通量表（PACS）和青少年心理韧性量表（RSCA）评估变化。试用结果显示，产品与家庭沟通质量提升、青少年复原力改善及家庭对家庭会议接受度提高存在积极关联；但受样本规模等限制，结论仍需在更大样本与更长期研究中进一步验证。  
The research conducted pre- and post-testing with 25 pilot families, using the Parent-Adolescent Communication Scale (PACS) and the Resilience Scale for Chinese Adolescents (RSCA). The pilot results suggest positive associations with improved family communication quality, adolescent resilience, and acceptance of family meetings. Given the sample-size and other limitations, these findings require validation through larger and longer-term studies.

**关键词 / Keywords：** 青少年心理健康 / Adolescent mental health；AI 家庭顾问 / AI Family Counselor；青少年复原力 / Adolescent resilience；家庭沟通质量 / Family communication quality；家庭会议 / Family meeting

## 项目结构 / Project Structure

```text
AI家庭顾问 / AI_Family_Consultant
├── AIFamilyConsultant_NewBackend_runable/   # Spring Boot 后端 / Spring Boot backend
├── AIFamilyConsultant_NewFrontend_User/     # 聊天前端 / Chat frontend
├── AIFamilyConsultant_NewFrontend_Admin/    # 后台管理前端 / Admin frontend
└── README.md
```

## v1.2.0 更新说明 / What's New in v1.2.0

- 整合后端、聊天前端和后台管理前端三个部分至同一总仓库，并通过 Git Submodule 保留各项目独立版本历史。  
  Integrated the backend, chat frontend, and admin frontend into one parent repository while retaining each project's independent history through Git submodules.
- 聊天前端与后台管理前端补充了主要交互文案、导航、筛选项、表头及操作按钮的中英双语显示。  
  Added Chinese-English bilingual labels to key interface copy, navigation, filters, table headers, and action buttons in the chat and admin frontends.
- 完善项目 README，使项目介绍、研究背景、能力说明、技术信息和版本记录均提供中英文内容。  
  Expanded this README so that the project overview, research background, capabilities, technical details, and release history are available in both Chinese and English.

## 技术说明 / Technology Stack

- 后端 / Backend：Java / Spring Boot
- 聊天前端 / Chat frontend：React / Vite
- 后台管理前端 / Admin frontend：React / Umi Max
- 数据库 / Database：MySQL
- 缓存 / Cache：Redis
- 大语言模型 / Large language models：通过后台模型管理配置并调用 / Configured and invoked through the admin model-management interface

## 版本记录 / Version History

- `v1.2.0`：整合三个项目至总仓库；补充 User/Admin 端主要中英双语界面；完善双语 README。  
  Integrated the three projects into the parent repository; added key bilingual UI content to User/Admin; completed the bilingual README.
- `v1.1.0`：新增可视化模型管理，并支持分别配置聊天模型与报告模型。  
  Added visual model management and support for separate chat and report model configuration.
- `v1.0.0`：首次发布的基础版本。  
  Initial baseline release.
