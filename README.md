# Requirement Translator

AI 輔助的跨角色需求轉譯工具雛形。

## 專案簡介

Requirement Translator 是一個以 PM 與系統分析角色為出發點所設計的需求轉譯原型，目的是協助使用者辨識模糊需求、整理待確認資訊，並將較口語化的客戶需求，轉化為較具結構的技術討論內容。

在跨部門協作中，客戶、PM 與工程師往往站在不同角色與專業背景下理解同一個需求，因此容易產生資訊落差、理解不一致，甚至影響後續實作。

這個專案希望處理的是「如何讓不同角色更清楚地理解彼此」。

## 問題情境

客戶提出的需求，常常會包含較模糊或主觀的描述，例如：

- 「希望系統快一點」
- 「操作可以更方便」
- 「最好不要每次都輸入密碼」

這些表達在溝通上可以被理解，但對工程實作而言，仍缺乏明確且可驗證的條件。

因此，系統不直接替使用者假設答案，而是先辨識模糊資訊，再提出需要進一步確認的問題。

## 核心流程

Client Requirement  
→ Requirement Analysis  
→ Ambiguity Detection  
→ Clarification Questions  
→ Human Input  
→ Refined Acceptance Criteria

也就是：

原始需求  
→ 需求分析  
→ 模糊點辨識  
→ 產生澄清問題  
→ 人工補充資訊  
→ 形成較具體的驗收條件

## 主要功能

- 區分 Functional Requirements 與 Non-functional Requirements
- 辨識模糊或主觀描述
- 產生 Questions to Clarify
- 提供 PM View
- 提供 Engineer View
- 產生 User Story
- 產生 Acceptance Criteria
- 支援 Clarification / Refine 流程
- 顯示 Before / After 對照
- 顯示 Confidence Level
- 保留 Human Review Required 提醒

## 範例

### Before

> 我希望會員登入可以快一點，而且不要每次都輸入密碼。

### Clarification

- 登入時間：2 秒內
- 登入方式：Google / Apple login
- Session：30 天

### After

- 登入流程應於 2 秒內完成。
- 系統應支援 Google 或 Apple 第三方登入。
- 登入狀態可保存最多 30 天。

## 人機協作方式

本專案為人機協作成果。

AI 工具協助我完成部分程式實作與debug，而我主要負責：

- 問題定義
- 需求設計
- 功能流程設計
- 資訊架構
- 介面方向
- 功能取捨
- 測試與修正

對我而言，AI 並不是替我完成整個專案，而是協助我把原本較模糊的想法，轉化成可以實際操作與測試的 prototype。

## 為什麼做這個專案

我關注的研究問題之一，是不同專業角色之間如何進行需求理解與資訊轉譯。

尤其在企業專案情境中，PM 經常需要在客戶端的商業需求與工程端的技術限制之間進行溝通與協調。

因此，我希望透過 Requirement Translator，初步探索資訊科技與 AI 是否能協助整理需求、辨識資訊落差，並支援跨角色溝通。

## 未來可延伸方向

- 串接生成式 AI 模型
- 支援更複雜的企業需求情境
- 產生結構化 Requirement Specification
- 增加需求版本追蹤
- 支援多角色協作
- 匯出需求文件
- 加入更多產業情境與測試案例

## Live Demo

https://violet720.github.io/Requirement-Translator/
