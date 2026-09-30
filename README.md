# Requirement Translator

AI 輔助的跨角色需求轉譯工具雛型。

## 專案說明

Requirement Translator 是一個以 PM 與系統分析情境為出發點所設計的需求轉譯雛型。

專案主要處理的問題，是客戶、PM 與工程端在需求溝通過程中，可能因角色與專業背景不同，而對同一句需求產生不同理解。

例如：

- 希望系統快一點
- 操作可以更方便
- 最好不要每次都輸入密碼

這些需求在溝通上可以理解，但若要進一步交付工程端實作，仍需要補充更明確的條件。

因此，本工具的設計重點不是直接替使用者補完需求，而是先辨識模糊資訊，提出需要確認的問題，再透過人工補充逐步形成較具體的需求內容。

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

- Functional Requirements 分類
- Non-functional Requirements 分類
- Ambiguity Detection
- Questions to Clarify
- PM View
- Engineer View
- User Story
- Acceptance Criteria
- Clarification / Refine 流程
- Before / After 對照
- Confidence Level
- Human Review Required 提醒

## 操作範例

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

## 專案角色與實作方式

本專案採人機協作方式完成。

AI 工具協助部分程式實作與除錯，我主要負責：

- 問題定義
- 需求流程設計
- 資訊架構規劃
- PM / Engineer 視角設計
- 功能取捨
- 使用情境測試
- 介面調整與修正

專案開發過程中，我特別關注的是如何將模糊需求逐步轉化為可以被不同角色共同理解與討論的資訊。

## 專案與研究興趣的關係

這個雛型與我目前關注的研究方向有直接關聯。

我希望進一步理解，在跨專業合作情境中，PM 如何在客戶需求與工程規格之間進行資訊轉譯，以及 GenAI 是否能在需求整理、資訊理解與跨角色溝通中提供協助。

Requirement Translator 是我將這個問題先轉化為實作雛型的一次嘗試。

## 未來規劃

後續希望進一步加入：

- 生成式 AI 模型串接
- 更複雜的企業需求案例
- 結構化 Requirement Specification
- 需求版本紀錄
- 文件匯出
- 多角色協作情境

## Live Demo

https://violet720.github.io/Requirement-Translator/
