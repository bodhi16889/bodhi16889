# 姚季緯 · Adan Yao

**FinTech 品質工程 18 年 → AI 應用開發**｜LLM 落地、Agent 流程、自動化測試架構

目前在愛金卡（icash Pay）擔任測試專案經理，近三年把 AI 從 PoC 推進到「團隊每天在用」的流程：
本地 LLM 推論環境（WSL2 + Ollama）、AI Agent 自動解析 API 規格並生成／修復測試腳本、
AI Code Review 關卡、團隊知識庫、AI 日誌分類。同時自研內部工具（Flutter 支付模擬 App、
Node.js POS 輔助工具、Python 自動化框架整合 C# 加密核心）。

我的驗收標準很單純：**能不能被別人重跑、能不能被追問數字。**

---

## 代表作品

### [trading-gates](https://github.com/bodhi16889/trading-gates) · Python
交易決策閘門層：append-only JSONL 決策帳本 + fail-closed 自測 + 事後回驗。
重點在三層分離（推理／確定性閘門／執行）與「取不到資料一律 BLOCK」的紀律，
不是交易策略。附 10 項零依賴離線斷言：

```
$ python3 test_decision_gates.py     # 不連網
PASS  全部資料失敗不得靜默
PASS  資料失敗必須入帳
SELFTEST PASS
```

### [fly-swat-rampage](https://github.com/bodhi16889/fly-swat-rampage) · Canvas 2D / H5
單檔 HTML5 遊戲（100 關／20 武器），符合 GamePix SDK v3 上架規範：
手動生命週期、廣告包裝、640×480 iframe、ZIP 只含 `index.html`。
附 100 項 Playwright 端到端驗證（含像素指紋比對與迴歸案例）。

▶ [線上試玩](https://bodhi16889.github.io/fly-swat-rampage/)

### [iAppium_python_cp2](https://github.com/bodhi16889/iAppium_python_cp2) · Python / Appium
Android 自動化測試框架（Appium + Python），含 Page Object 分層與 Allure 報告。

---

## 未公開的內部專案（金融資安規範）

下列是我在職期間自研、但**依公司資安規範不得公開程式碼**的內部工具與平台。
原始碼留在內部私有 repo，作品以「架構＋可驗證指標」呈現，面試時可現場 demo：

| 專案 | 內容 | 成果指標 |
|---|---|---|
| AI Agent 測試生成流程 | 「資料／生成／執行」三層分離：解析 API 規格 → 生成測試腳本 → 自我修復 | 腳本維護成本 −30%、首版通過率 +35% |
| AI Code Review Gate | 上版前的強制檢查點，以歷史缺陷資料做規則式缺陷預測 | 缺陷提前攔截率 95% |
| 團隊 AI 知識庫 | 測試規範、API 規格、歷史修復案例的可檢索知識資產 | 新人上手與重複排查時間下降 |
| 支付情境模擬工具（Flutter） | 手機端一鍵模擬 POS／超商／跨境等 7 種支付情境，取代多段 Postman 呼叫 | 測試前置作業由數十分鐘降至分鐘級 |
| API 自動化框架 | Python 框架整合 C# 加密核心，Jenkins 產出數位化報告 | 200+ 支腳本、每日回歸 |
| AI 日誌分類 | 密集 UAT 期自動分類 Error Log 並聚類 | RCA 時間 −50% |

> 公開版以可驗證的等價作品呈現（如 [trading-gates](https://github.com/bodhi16889/trading-gates)
> 即為同一套「fail-closed ＋ append-only 帳本」方法論的去識別化版本）。

---

## 技術範圍

**AI / LLM**　Ollama、Gemma、Hermes、Claude Code、GitHub Copilot Enterprise、
Prompt Engineering、Agent 流程設計、MCP、LLM 評測（Evals / Benchmark）、
AI Code Review、提示注入防護、Red Teaming

**語言**　Python、C#、Node.js、Dart / Flutter、Java、SQL、JavaScript

**測試與自動化**　PyTest、Selenium、Appium、Playwright、JMeter（分散式壓測）、Locust、
Postman、Katalon、Airtest

**平台**　Jenkins、GitLab CI/CD、Git、Docker / WSL2、Jira、Redmine、Figma、
GitHub Pages、Slack

**領域**　電子支付（icash Pay）、第三方金流（ECPay）、網通 / IoT（D-Link）

---

## 經歷

| 期間 | 角色 |
|---|---|
| 2023/01 – 現在 | 愛金卡 icash Pay｜測試專案經理 |
| 2022/10 – 2023/01 | 酷遊天｜資深測試工程師（短期專案） |
| 2019/04 – 2022/09 | 綠界科技 ECPay｜測試主任 |
| 2006/06 – 2018/04 | 友訊科技 D-Link｜測試驗證部副理 / 專案副理 |

📧 adanyao@gmail.com
