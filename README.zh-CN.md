<!-- 此中文譯本對應英文權威文件：[`README.md`](README.md)。如有差異，以英文版為準。 -->

# Jekyll 學習檔案庫

這是一個雙語、以 Jekyll 為先的刻意練習和自主學習檔案庫。每份學習紀錄都是 post，所以網站本身就是資料庫，而不是另一份本機資料夾匯出。

## 從這裡開始

1. 閱讀 [AGENTS.md](AGENTS.md)，了解 agent 必須遵守的規則。
2. 開啟網站的 **Categories**、**Tags** 和 **Archives** 分頁瀏覽資料庫。
3. 開始學習會談前，先閱讀 current-goal 和 learner-context post。

## 內容資料庫

所有學習 Markdown 都存於 `_posts/<record-type>/`。Post 資料夾和 `record_type` 用來識別紀錄種類；`categories` 則提供 Jekyll Categories 頁面所顯示的精簡兩層導航。第一個 category 是群組，第二個是其子 category。不可加入第三層；更細的區分使用 tag。

| Category 群組 | 子 categories | 紀錄種類／資料夾 |
|---|---|---|
| `goals` | — | 目標和成果：`_posts/goals/` |
| `notes` | `ideas`、`thinking`、`reflections`、`distilled` | 擷取、學習者推理、反思和可重用知識：`_posts/ideas/`、`_posts/thinking/`、`_posts/reflections/`、`_posts/knowledge/` |
| `practice` | `active-drills`、`attempts`、`feedback`、`scorecards` | 刻意練習規格和證據：`_posts/drills/`、`_posts/attempts/`、`_posts/feedback/`、`_posts/scorecards/` |
| `docs` | `learner-context`、`templates` | 學習者 profile／現況和可重用紀錄結構：`_posts/learner-context/`、`_posts/templates/` |
| `sources` | `references` | 來源紀錄、引用筆記和已批准的參考材料：`_posts/sources/` |
| `log` | `daily`、`raw-history` | 每日會談紀錄和有意保留的原始追蹤紀錄：`_posts/logs/`、`_posts/raw-history/` |
| `reviews` | — | 每日、每週或每月綜合：`_posts/reviews/` |

每篇英文權威 post 都有同資料夾內的中文對應檔：

```text
_posts/knowledge/2026-09-17-topic.md
_posts/knowledge/2026-09-17-topic.zh-CN.md
```

Post 使用明確的英文和中文 permalink、路由表指定的 category 階層，以及較窄的主題 tag。以 permalink 連結 post，以 `/Diagrams/` 連結視覺資產；不可再使用舊工作區資料夾的相對連結。

## 建立紀錄

在相應的 record-type 資料夾內，同時建立英文和中文 post。使用 `AGENTS.md` 訂明的必填 front matter：title、date、permalink、categories、tags、description、comments、table-of-contents setting、language、translation key 和 record type。

此 repository 按設計就是公開網站內容。不可在 post 放入憑證、私密 token、敏感個人資料，或未獲批准的受版權保護逐字稿。

## 技術檔案

Root 只保留網站需要的操作檔：agent 指示、本指南、Jekyll 設定、dependencies、deployment workflow、site tabs、plugins、assets 和 diagrams。學習文件不應再放在獨立的 root-level 內容資料夾。
