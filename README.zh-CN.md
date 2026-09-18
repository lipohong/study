<!-- 此中文譯本對應英文權威文件：[`README.md`](README.md)。如有差異，以英文版為準。 -->

# Jekyll 學習檔案庫

這是一個雙語、以 Jekyll 為先的刻意練習和自主學習檔案庫。每份學習紀錄都是 post，所以網站本身就是資料庫，而不是另一份本機資料夾匯出。

## 從這裡開始

1. 閱讀 [AGENTS.md](AGENTS.md)，了解 agent 必須遵守的規則。
2. 開啟網站的 **Categories**、**Tags** 和 **Archives** 分頁瀏覽資料庫。
3. 開始學習會談前，先閱讀 current-goal 和 learner-context post。

## 內容資料庫

所有學習 Markdown 都存於 `_posts/<record-type>/`。每篇 post 只有一個頂層 category，用來表示其角色並驅動 Jekyll 的 category view。

| Category | 內容 |
|---|---|
| `goals` | 目前目標、長期目標和拆解 |
| `learner-context` | 學習者 profile 和目前學習狀態 |
| `knowledge` | 可重用概念、模型、解釋和圖表 |
| `ideas`、`thinking`、`reflections` | 擷取、學習者推理和反思 |
| `drills`、`attempts`、`feedback`、`scorecards` | 刻意練習證據 |
| `sources` | 來源紀錄和引用筆記 |
| `logs`、`reviews` | 按時間排序的會談歷史和綜合 |
| `templates` | 可重用 post 結構 |

每篇英文權威 post 都有同資料夾內的中文對應檔：

```text
_posts/knowledge/2026-09-17-topic.md
_posts/knowledge/2026-09-17-topic.zh-CN.md
```

Post 使用明確的英文和中文 permalink、穩定的 category，以及較窄的主題 tag。以 permalink 連結 post，以 `/Diagrams/` 連結視覺資產；不可再使用舊工作區資料夾的相對連結。

## 建立紀錄

在相應的 record-type 資料夾內，同時建立英文和中文 post。使用 `AGENTS.md` 訂明的必填 front matter：title、date、permalink、categories、tags、description、comments、table-of-contents setting、language、translation key 和 record type。

此 repository 按設計就是公開網站內容。不可在 post 放入憑證、私密 token、敏感個人資料，或未獲批准的受版權保護逐字稿。

## 技術檔案

Root 只保留網站需要的操作檔：agent 指示、本指南、Jekyll 設定、dependencies、deployment workflow、site tabs、plugins、assets 和 diagrams。學習文件不應再放在獨立的 root-level 內容資料夾。
