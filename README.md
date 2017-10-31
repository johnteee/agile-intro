Agile簡介&經驗分享
==

---

# 什麼是Agile?

---

Agile = Concurrent Engineering + Lean

---

## Concurrent Engineering:

  * 合作交流、資訊透明、自我組織 (不是新東西)

http://www2.nkfust.edu.tw/~jcyu/ConcurrentEngineering/ConcurrentEngineeringIndex.htm

---

## Lean:

  * 減少浪費、降低風險、持續改善、價值導向

---

# 實際作法的介紹(以Scrum為例子)

---

## Agile的作法千百種，以Scrum作一個例子簡介

---

## Agile重視團隊的文化及運作模式，而角色各有著重:
  * Stakeholder
  * ProductOwner
  * ScrumMaster
  * TeamMember

---

## Stakeholder:
  * 利益相關者，可能是老闆或業務部門

---

## ProductOwner:
  * 必須承擔產品成敗的風險
  * 依照決定feature被執行的優先序(依照Value與成本)
  * 與客戶溝通需求及紀錄

---

## ScrumMaster:
  * 維護/引導團隊運作流程
  * Team Building
  * 打雜/文書紀錄

---

## TeamMember:
  * 協助PO規劃時程及技術成本(時間&人員&錢)
  * 告知PO現實情況，反映實務上的問題
  * 有效率執行工作

---

## 必要活動:
  * RequirementWorkshop( Stakeholder&PO )
  * RefinementWorkshop( PO&TeamMember )
  * IterationPlanning( PO&TeamMember )
  * DailyScrum( PO&TeamMember )
  * Demo/Review( Stakeholder&PO&TeamMember )
  * Retrospective( PO&TeamMember )

---

## RequirementWorkshop:
  * PO與客戶討論Feature細節
  * PO與客戶記下驗收的準則(DefinitionOfDone)
  * PO得到Feature的Business Value

---

## RefinementWorkshop:
  * PO與團隊成員討論Feature細節
  * 成員給出每個Feature大概的執行成本(技術&錢&時間&人力)
  * 成員將Scope太大的Feature切割，變成很多個單次iteration可以執行的feature單位(漸進式)
  * PO確認無誤，將Feature加入Backlog

---

## -> ProductOwner的需求優先度管理:
  * PO由**RequirementWorkshop**與**RefinementWorkshop**得知Feature的**BusinessValue**&**成本**
  * PO以此兩個數值作為依據給出Priority值來作為優先度依據

---

## IterationPlanning:
  * 由團隊成員一起切出各Feature實際最小單位task並估算成員時間
  * 統計該次Iteration最多可以作到幾個Feature，包括人力配置及請假(因為Scrum是iteration/release based)
  * PO依Priority及人力對Feature作出取捨

---

## -> 執行工作時:
  * 成員要一起將最難的部份解決再開始下一個Feature，以免有Feature更重要卻遲遲卡關
  * 若有時間同時也能培養多能工, PairProgramming

---

## DailyScrum:
  * 簡潔，同步大家工作進度及項目狀態
  * 避免太短或太長，困難的點要點出來以及需要的人手及資源等等

---

## Review/Demo:
  * 避免過長時間才作Review，即早與客戶確認需求是必須的
  * 若需求已滿足DefinitionOfDone則可以找客戶來Review，未必要等到iteration結束

---

## Retrospective:
  * 提出改善流程的建議
  * 必須是具體改善事項及作法，對事不對人

---

## -> 除此之外，還需要一些輔助
  * 知識共享(類似Wiki等非正式內部文件知識交流系統)
  * 自動化工具(DevOps&VCS)及電子化追蹤紀錄(Slack+Trello...etc)
  * 多能工的培養

---

## -> 沒有多能工的能力怎麼辦?
  * PairProgramming & Dojo(道場)
  * 簡單工作交給不同專業的人來嘗試實作
  * 駭客文化的風氣

---

## -> 重要的執行細節:
  * 按Priority執行並減少半成品的發生
  * DefinitionOfDone(驗收成果)
  * 資訊透明化及自動化(讓問題浮現並減少人為疏失)
  * 即時的需求與成果確認(減少作出不被需要的成品)

---

# 開發流程的理想制度

---

## 需求管理
  * 由PO與客戶在RequirementWorkshop
    * 進行溝通Feature，並紀錄驗收的Criteria
    * 決定BusinessValue
  * 由PO與團員在RefinementWorkshop
    * 進行每個Feature的時間人力金錢成本預估
    * 將過大無法執行的工作，切割成可以執行並驗收的最小階段性目標(一個大feature->很多個可以分階段完成的feature)
    * 決定這個工作的成本Cost
  * 由PO透過BusinessValue和Cost進行決斷，並得出Priority進行優先度的決定

---

## 工作排程
  * 團員: 以Priority高的feature先被完成為基準，再進行下一個feature(減少什麼都作一半而產生一堆半成品的情況)
  * PO與客戶間的溝通很重要，並且PO是關鍵的人物(什麼要作什麼不要作，客戶怎樣才會滿意<-客戶真正想要的東西，客戶的需求細節理解等等)
  * 插件工作的情況必須給予Priority值，不能太隨意插件

---

## 風險管理
  * Internal Refactoring必須佔工作排程上一定比例，讓軟體品質能夠更有效的被維護
  * DefinitionOfDone必須被有效驗證才能視為完成工作，減少執行沒有完成的情況
  * 及早整合程式碼並測試(例如: Client-Server兩方的互動串接)
  * 自動化Dashboard等數值以及實踐DevOps，減少工程師及OP團隊的人力浪費
  * 透明化&電子化工作進度及項目，讓每個人都能得知狀態，減少互相等待的浪費

---

## 改善會議
  * 提出改善流程的建議
  * 必須是具體改善事項及作法
  * 對事不對人

---

## 軟體品質管理
  * SmokingTest的落實(服務的重要運作流程整合測試，至少要作到HappyPath)
  * 單元測試的落實(雖然不強求coverage 100%，但是至少一些重要邏輯/流程都要有測試)
  * 程式碼可測化(Refactor 程式)
  * 善用Test Double
    * Dummy 求編過可以Run的物件
    * Fake 改寫少數Func的真物件
    * Stub 被測的資料(提供測試需要的資料)
    * Spy 紀錄並提供自身被操作的過程的真物件
    * Mock 預定義行為及資料的假物件

---

## Cross Functional Team
  * Mentor 機制
  * Job Rotation 機制

---

### Mentor 機制
  * 各專長的人們可以定期排定Dojo(作中學)及用以PairProgramming的工作項目，找有興趣的人們來參與
  * WIKI紀錄各個專業專案的初始化Know-How及環境Settings

---

### Job Rotation 機制
  * 以 cross functional team 為目標(每個人都會一點，然後pair programming的方式資深者來帶初學者)
  * 可能要看每個人自己想要訓練的第二專長為主，然後將來開一些Dojo的Hackthon來作一些基礎訓練。 (像是公司內部社團及研討會的方式，比較看個人的意願)
  * 以制度化這樣的跨領域學習文化，然後進一步去領跨領域的工作(Pair Programming)

---

## Issue Tracking & Bug Report
  * issue與對應Feature作Link
  * 自動在Git Commit時WebHook，把電子白板的issue上自動加上CommitId的Comment，以提供追蹤
  * issue必須紀錄以下資訊以利追蹤:
    * 軟體版本
    * 發生環境及裝置
    * 重現步驟
    * Screenshot & Video & 描述

---

# Q & A
