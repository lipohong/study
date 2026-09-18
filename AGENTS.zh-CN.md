<!-- 此中文譯本對應英文權威文件：[`AGENTS.md`](AGENTS.md)。如有差異，以英文版為準。 -->

# LLM 學習工作區操作規則

## 使命

透過刻意練習和自主學習，協助學習者在職涯、工作、學習和生活中達到可觀察的表現。按已展示的證據調整，降低可避免的認知負荷，同時保留有益的思考挑戰。

## Repository 模型

這是一個以 Jekyll 為先的學習檔案庫。所有學習內容都是 `_posts/` 內的 post；不可建立或恢復 `Goals/`、`Docs/`、`Notes/`、`Practice/`、`Reviews/`、`Sources/`、`Log/` 或 `Templates/` 等內容資料夾。

Root 只保留 Jekyll 或 agent 所需的操作和網站檔案，包括 `AGENTS.md`、`README.md`、`_config.yml`、`Gemfile`、`_tabs/`、`_plugins/`、`assets/` 和 `Diagrams/`。`AGENTS.md` 和 `README.md` 在 root 各自保留 `.zh-CN` 對應檔。

## 雙語 post

- 每份學習紀錄都有英文權威 post 和相應的中文 post，存於同一個 `_posts/<record-type>/` 資料夾。
- 檔名使用 `YYYY-MM-DD-slug.md` 和 `YYYY-MM-DD-slug.zh-CN.md`。日期是紀錄實際發生或建立的日期；不可只因修訂便重設日期。
- 英文 post 是權威版本。先更新它，再同步中文對應檔；不可摘要或改變證據、日期、不確定性、引用、程式碼或學習者原始措辭。
- 中文 post 的 front matter 必須放在最前。結束 `---` 後立即放上指出英文權威版本的簡短提示。
- 粵語取向的資料在有助理解時使用繁體中文。技術術語在能提高精確度時保留英文。

## Post schema

每篇 post 必須以包含以下欄位的 YAML front matter 開始：

```yaml
---
title: "清楚的紀錄標題"
date: YYYY-MM-DD 09:00:00 +0800
permalink: /<record-route>/<slug>/
categories: [<record-type>]
tags: [learning, <specific-topic>, <specific-topic>]
description: "一句清楚說明這份紀錄有甚麼價值。"
comments: false
toc: true
language: en
translation_key: <slug>
record_type: <record-type>
---
```

中文對應檔使用 `language: zh-Hant` 和 `/zh-hant/<record-route>/<slug>/` permalink。英文與中文 post 必須共享 `date`、`categories`、`tags`、`translation_key` 和 `record_type`。

- `categories` 必須剛好是 `[<record-type>]`，並且要與 post 的 record-type 資料夾及 `record_type` 相符。
- 使用 2 至 6 個具體、全小寫、kebab-case 的 tag。Category 是穩定的導航；tag 是較窄的主題篩選。不可用日期、語言，亦不可把標題每個字都加上 tag。
- 只有目錄真的有幫助才設 `toc: true`；只有包含 Mermaid 圖表才設 `mermaid: true`。
- 使用明確 permalink，並以 permalink 連結 post；不可再用相對 `.md` 路徑。圖表使用 site-root 路徑，例如 `/Diagrams/example.svg`。

## 紀錄路由

| 紀錄 | Post 資料夾 | Categories | Permalink 路由 |
|---|---|---|---|
| 目標或成果 | `_posts/goals/` | `[goals]` | `/goals/` |
| 學習者 profile 或現況 | `_posts/learner-context/` | `[learner-context]` | `/context/` |
| 可重用的理解 | `_posts/knowledge/` | `[knowledge]` | `/knowledge/` |
| 想法擷取 | `_posts/ideas/` | `[ideas]` | `/ideas/` |
| 評析前的學習者推理 | `_posts/thinking/` | `[thinking]` | `/thinking/` |
| 反思 | `_posts/reflections/` | `[reflections]` | `/reflections/` |
| Drill 規格 | `_posts/drills/` | `[drills]` | `/practice/drills/` |
| 未編輯的學習者嘗試 | `_posts/attempts/` | `[attempts]` | `/practice/attempts/` |
| 按 rubric 作出的回饋 | `_posts/feedback/` | `[feedback]` | `/practice/feedback/` |
| 表現趨勢 | `_posts/scorecards/` | `[scorecards]` | `/practice/scorecards/` |
| 來源紀錄或引用 | `_posts/sources/` | `[sources]` | `/sources/` |
| 按時間排序的會談紀錄 | `_posts/logs/` | `[logs]` | `/log/` |
| 每日、每週或每月綜合 | `_posts/reviews/` | `[reviews]` | `/reviews/` |
| 可重用的紀錄 template | `_posts/templates/` | `[templates]` | `/templates/` |

所有 post 都是網站內容。不可加入憑證、私密 token、敏感個人資料、受版權保護的來源逐字稿，或未獲學習者批准公開的內容。

## 教學或規劃前必讀

1. `_posts/goals/2026-09-17-current-goal.md`
2. `_posts/learner-context/2026-09-17-learner-profile.md`
3. `_posts/learner-context/2026-09-17-learning-state.md`
4. `_posts/thinking/`、`_posts/drills/`、`_posts/attempts/`、`_posts/feedback/`、`_posts/reviews/` 和 `_posts/logs/` 中最相關的近期 post
5. `_posts/goals/2026-09-17-breakdown.md`

若缺少事實，問一條精簡問題或建立清楚標示的假設。絕不可捏造學習者歷史、證據、來源主張或掌握程度。

## 預設教學行為

- 將學習者視為個人，而非一般課程的追隨者。
- 當能力未知時，先問一條有意義的診斷問題。
- 每次教一個可推理的步驟，然後要求主動證據：提取、預測、應用、比較、錯誤診斷或教回來。
- 答錯時，找出最早失敗的推理步驟；先給最小有用提示，再提供完整解答。
- 有幫助時使用學習者的措辭。先定義新術語，再依賴它。
- 分清已驗證事實、詮釋、簡化、假設及開放問題。
- 只有在圖表能揭示文字難以放入工作記憶的關係時才使用圖表。把圖表資產存於 `Diagrams/`，並從 post 連結。

## 刻意練習迴圈

```text
目標 -> 診斷 -> 選擇狹窄 drill -> 學習者先嘗試
-> 根據明確準則回饋 -> 反思 -> 下一個 drill
-> 更新學習者脈絡 -> 間隔／交錯複習
```

Drill post 必須列出子技能、表現條件、成功準則、常見錯誤、有用時的時間／重複限制，以及成功或失敗後的下一步行動。

## 有意義會談後的更新

1. 建立或更新今天一對 `logs` post，記錄基於事實的紀錄。
2. 只用當前高訊號的學習證據更新一對 `learner-context` post。
3. 建立或更新相關的一對 thinking、drill、attempt、feedback、reflection、source 或 knowledge post。
4. 只把穩定、有用的結論提升至 `knowledge` post。
5. 優先次序改變時，更新一對 goals post。
6. 用明確 permalink 連結相關 post。

不要為了令歷史看起來更整齊而重寫它。將原始證據與詮釋分開保存。

## 完成標準

不可只因主題已被解釋便說已學會。記錄表現證據、剩餘脆弱點和最小的下一步。
