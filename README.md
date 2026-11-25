
# Requirement Translator
### 需求轉譯與澄清輔助工具

> From Ambiguous Requests to Clear Requirements.  
> 從模糊需求出發，建立更清晰的需求共識。

## 01. Project Overview｜專案概述

Requirement Translator 是一項以需求工程（Requirements Engineering）為核心的系統雛型，旨在協助專案經理（PM）與工程師釐清需求描述中的模糊資訊，降低不同角色之間的理解落差。

本專案採用規則式需求分析方法，透過模糊詞辨識、澄清問題及需求整理，探索如何將原始需求轉換為更明確、可供討論的系統規格。

**Core Principle：Clarify Before Implementing.**

先確認使用者真正的需求，再評估適當的技術方案。

## 02. Problem Statement｜問題定義

在資訊系統開發過程中，客戶、PM 與工程師可能因專業背景、工作職責及資訊掌握程度不同，對同一項需求產生不同理解。

本專案關注三項問題：

### P-01｜需求描述模糊
使用者常以「方便」、「快速」、「安全」等主觀詞彙表達需求，卻缺乏明確的衡量標準。

### P-02｜潛在限制未被充分辨識
需求可能涉及資料權限、業務流程、技術限制與例外情況，但這些條件未必會在初次溝通時提出。

### P-03｜需求確認機制不足
缺乏明確的需求確認與驗收依據，可能增加反覆溝通、重工及專案延遲的風險。

## 03. Project Objectives｜專案目標

本專案希望透過結構化的需求分析流程：

1. 協助辨識需求描述中的模糊資訊。
2. 提供澄清問題，支持 PM 與客戶的需求討論。
3. 協助整理不同角色對需求的理解。
4. 探索需求完整性檢查與人工確認機制。
5. 降低需求資訊不足所造成的專案風險。

上述目標包含目前雛型的既有方向，以及後續規劃，並不代表所有功能均已完成。

## 04. Target Users｜目標使用者

| 使用者 | 主要需求 |
|---|---|
| Project Manager | 釐清客戶需求、降低溝通落差 |
| System Analyst | 分析需求、整理規格與限制 |
| Software Engineer | 理解業務需求與技術條件 |

## 05. Current Prototype｜現階段雛型

目前專案以瀏覽器端的規則式文字分析為基礎，包含：

- 原始需求輸入
- 模糊需求辨識
- 澄清問題產生
- PM View / Engineer View
- User Story 與 Acceptance Criteria 整理
- 初步需求補充流程

目前的分析能力受到預先設定的文字規則限制，尚無法完整理解所有自然語言情境。

## 06. System Workflow｜系統流程

原始需求輸入
→ 模糊資訊辨識
→ 澄清問題產生
→ 人工補充
→ 需求規格整理

此流程為目前雛型的概念摘要，後續將補充詳細架構圖與設計文件。

## 07. Demo｜線上展示

[Live Demo](https://violet720.github.io/Requirement-Translator/)

## 08. Documentation｜專案文件

後續預計建立：

- Problem Analysis｜問題分析
- Stakeholder Analysis｜利害關係人分析
- Requirements Specification｜需求規格
- System Design｜系統設計
- Testing & Validation｜測試與驗證

## 09. Limitations & Roadmap｜限制與未來規劃

### Current Limitations
- 規則式分析的語意理解能力有限。
- 尚缺乏系統性的測試結果。
- 需求完整性與風險判斷仍需深化。

### Future Development
- 需求完整性檢查
- 需求風險提示與優先排序
- 人工確認及狀態紀錄
- 更完整的驗收條件產生機制
- 探索整合生成式 AI 的可行性

## 10. Reflection｜專案反思

本專案從 PM 與工程師的需求認知落差出發，嘗試將需求管理中的問題轉化為可操作的資訊工具。

開發過程中，持續思考如何在技術實作之前釐清使用者需求，並透過需求工程方法改善資訊傳遞與跨角色協作。
