<p align="center">
  <img src="assets/TauricResearch.png" style="width: 60%; height: auto;">
</p>

<div align="center" style="line-height: 1;">
  <a href="https://arxiv.org/abs/2412.20138" target="_blank"><img alt="arXiv" src="https://img.shields.io/badge/arXiv-2412.20138-B31B1B?logo=arxiv"/></a>
  <a href="https://discord.com/invite/hk9PGKShPK" target="_blank"><img alt="Discord" src="https://img.shields.io/badge/Discord-TradingResearch-7289da?logo=discord&logoColor=white&color=7289da"/></a>
  <a href="./assets/wechat.png" target="_blank"><img alt="WeChat" src="https://img.shields.io/badge/WeChat-TauricResearch-brightgreen?logo=wechat&logoColor=white"/></a>
  <a href="https://x.com/TauricResearch" target="_blank"><img alt="X Follow" src="https://img.shields.io/badge/X-TauricResearch-white?logo=x&logoColor=white"/></a>
  <br>
  <a href="https://github.com/TauricResearch/" target="_blank"><img alt="Community" src="https://img.shields.io/badge/Join_GitHub_Community-TauricResearch-14C290?logo=discourse"/></a>
</div>

<div align="center">
  <!-- Keep these links. Translations will automatically update with the README. -->
  <a href="https://www.readme-i18n.com/TauricResearch/TradingAgents?lang=de">Deutsch</a> | 
  <a href="https://www.readme-i18n.com/TauricResearch/TradingAgents?lang=es">Español</a> | 
  <a href="https://www.readme-i18n.com/TauricResearch/TradingAgents?lang=fr">français</a> | 
  <a href="https://www.readme-i18n.com/TauricResearch/TradingAgents?lang=ja">日本語</a> | 
  <a href="https://www.readme-i18n.com/TauricResearch/TradingAgents?lang=ko">한국어</a> | 
  <a href="https://www.readme-i18n.com/TauricResearch/TradingAgents?lang=pt">Português</a> | 
  <a href="https://www.readme-i18n.com/TauricResearch/TradingAgents?lang=ru">Русский</a> | 
  <a href="https://www.readme-i18n.com/TauricResearch/TradingAgents?lang=zh">中文</a>
</div>

---

# TradingAgents：多智能體 LLM 金融交易框架

## 最新消息

- [2026-03] **TradingAgents v0.2.3** 發布，新增多語言支援、GPT-5.4 系列模型、統一模型目錄、回測日期精確度提升及代理伺服器支援。
- [2026-03] **TradingAgents v0.2.2** 發布，涵蓋 GPT-5.4/Gemini 3.1/Claude 4.6 模型、五級評分量表、OpenAI Responses API、Anthropic 推理強度控制及跨平台穩定性改善。
- [2026-02] **TradingAgents v0.2.0** 發布，支援多供應商 LLM（GPT-5.x、Gemini 3.x、Claude 4.x、Grok 4.x）並改善系統架構。
- [2026-01] **Trading-R1** [技術報告](https://arxiv.org/abs/2509.11420) 發布，[終端程式](https://github.com/TauricResearch/Trading-R1)預計即將推出。

<div align="center">
<a href="https://www.star-history.com/#TauricResearch/TradingAgents&Date">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=TauricResearch/TradingAgents&type=Date&theme=dark" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=TauricResearch/TradingAgents&type=Date" />
   <img alt="TradingAgents Star History" src="https://api.star-history.com/svg?repos=TauricResearch/TradingAgents&type=Date" style="width: 80%; height: auto;" />
 </picture>
</a>
</div>

> 🎉 **TradingAgents** 正式發布！我們收到了大量關於本專案的詢問，非常感謝社群夥伴們的熱情支持。
>
> 因此我們決定將框架完全開源，期待與大家共同打造具有影響力的專案！

<div align="center">

🚀 [TradingAgents](#tradingagents-框架) | ⚡ [安裝與 CLI](#安裝與-cli) | 🎬 [示範影片](https://www.youtube.com/watch?v=90gr5lwjIho) | 📦 [套件使用](#tradingagents-套件) | 🤝 [貢獻指南](#貢獻指南) | 📄 [引用](#引用)

</div>

## TradingAgents 框架

TradingAgents 是一個多智能體交易框架，模擬真實交易公司的運作模式。透過部署專業化的 LLM 驅動智能體——從基本面分析師、情緒專家、技術分析師，到交易員與風險管理團隊——平台協同評估市場狀況並做出交易決策。此外，這些智能體還會進行動態討論，以找出最佳策略。

<p align="center">
  <img src="assets/schema.png" style="width: 100%; height: auto;">
</p>

> TradingAgents 框架專為研究用途設計。交易表現可能因多種因素而有所不同，包括所選擇的基礎語言模型、模型溫度、交易週期、資料品質及其他不確定因素。[本框架不構成任何財務、投資或交易建議。](https://tauric.ai/disclaimer/)

本框架將複雜的交易任務分解為專業化角色，確保系統以穩健、可擴展的方式進行市場分析與決策。

### 分析師團隊

- **基本面分析師**：評估公司財務狀況與績效指標，識別內在價值與潛在風險。
- **情緒分析師**：運用情緒評分演算法分析社群媒體與公眾輿論，衡量短期市場情緒。
- **新聞分析師**：監控全球新聞與總體經濟指標，解讀事件對市場狀況的影響。
- **技術分析師**：運用技術指標（如 MACD 和 RSI）偵測交易型態並預測價格走勢。

<p align="center">
  <img src="assets/analyst.png" width="100%" style="display: inline-block; margin: 0 2%;">
</p>

### 研究員團隊

- 由多頭與空頭研究員組成，對分析師團隊提供的洞察進行批判性評估。透過結構化辯論，在潛在收益與固有風險之間取得平衡。

<p align="center">
  <img src="assets/researcher.png" width="70%" style="display: inline-block; margin: 0 2%;">
</p>

### 交易員智能體

- 整合分析師與研究員的報告，做出知情的交易決策。根據全面的市場洞察決定交易的時機與規模。

<p align="center">
  <img src="assets/trader.png" width="70%" style="display: inline-block; margin: 0 2%;">
</p>

### 風險管理與投資組合經理

- 透過評估市場波動性、流動性及其他風險因素，持續評估投資組合風險。風險管理團隊評估並調整交易策略，向投資組合經理提供評估報告以供最終決策。
- 投資組合經理核准或拒絕交易提案。若核准，訂單將發送至模擬交易所並執行。

<p align="center">
  <img src="assets/risk.png" width="70%" style="display: inline-block; margin: 0 2%;">
</p>

## 安裝與 CLI

### 安裝

複製 TradingAgents 儲存庫：

```bash
git clone https://github.com/TauricResearch/TradingAgents.git
cd TradingAgents
```

在您常用的環境管理工具中建立虛擬環境：

```bash
conda create -n tradingagents python=3.13
conda activate tradingagents
```

安裝套件及其相依套件：

```bash
pip install .
```

### Docker

或者，使用 Docker 執行：

```bash
cp .env.example .env  # 填入您的 API 金鑰
docker compose run --rm tradingagents
```

使用 Ollama 執行本地模型：

```bash
docker compose --profile ollama run --rm tradingagents-ollama
```

### 必要 API

TradingAgents 支援多個 LLM 供應商。請為您選擇的供應商設定 API 金鑰：

```bash
export OPENAI_API_KEY=...          # OpenAI (GPT)
export GOOGLE_API_KEY=...          # Google (Gemini)
export ANTHROPIC_API_KEY=...       # Anthropic (Claude)
export XAI_API_KEY=...             # xAI (Grok)
export DEEPSEEK_API_KEY=...        # DeepSeek
export DASHSCOPE_API_KEY=...       # Qwen (阿里巴巴 DashScope)
export ZHIPU_API_KEY=...           # GLM (智譜)
export OPENROUTER_API_KEY=...      # OpenRouter
export ALPHA_VANTAGE_API_KEY=...   # Alpha Vantage
```

對於企業供應商（如 Azure OpenAI、AWS Bedrock），請將 `.env.enterprise.example` 複製為 `.env.enterprise` 並填入您的憑證。

對於本地模型，請在設定檔中以 `llm_provider: "ollama"` 配置 Ollama。

或者，將 `.env.example` 複製為 `.env` 並填入您的金鑰：

```bash
cp .env.example .env
```

### CLI 使用方式

啟動互動式 CLI：

```bash
tradingagents          # 已安裝的指令
python -m cli.main     # 替代方式：直接從原始碼執行
```

您將看到一個畫面，可在其中選擇所需的股票代碼、分析日期、LLM 供應商、研究深度等設定。

<p align="center">
  <img src="assets/cli/cli_init.png" width="100%" style="display: inline-block; margin: 0 2%;">
</p>

介面將顯示載入中的結果，讓您在智能體執行時追蹤其進度。

<p align="center">
  <img src="assets/cli/cli_news.png" width="100%" style="display: inline-block; margin: 0 2%;">
</p>

<p align="center">
  <img src="assets/cli/cli_transaction.png" width="100%" style="display: inline-block; margin: 0 2%;">
</p>

## TradingAgents 套件

### 實作細節

我們使用 LangGraph 建構 TradingAgents，以確保靈活性與模組化。框架支援多個 LLM 供應商：OpenAI、Google、Anthropic、xAI、OpenRouter 及 Ollama。

### Python 使用方式

若要在程式碼中使用 TradingAgents，您可以匯入 `tradingagents` 模組並初始化 `TradingAgentsGraph()` 物件。`.propagate()` 函式將回傳一個決策。您可以執行 `main.py`，以下是快速範例：

```python
from tradingagents.graph.trading_graph import TradingAgentsGraph
from tradingagents.default_config import DEFAULT_CONFIG

ta = TradingAgentsGraph(debug=True, config=DEFAULT_CONFIG.copy())

# 正向傳播
_, decision = ta.propagate("NVDA", "2026-01-15")
print(decision)
```

您也可以調整預設設定，自訂 LLM 選擇、辯論輪次等。

```python
from tradingagents.graph.trading_graph import TradingAgentsGraph
from tradingagents.default_config import DEFAULT_CONFIG

config = DEFAULT_CONFIG.copy()
config["llm_provider"] = "openai"        # openai, google, anthropic, xai, openrouter, ollama
config["deep_think_llm"] = "gpt-5.4"     # 用於複雜推理的模型
config["quick_think_llm"] = "gpt-5.4-mini" # 用於快速任務的模型
config["max_debate_rounds"] = 2

ta = TradingAgentsGraph(debug=True, config=config)
_, decision = ta.propagate("NVDA", "2026-01-15")
print(decision)
```

所有設定選項請參閱 `tradingagents/default_config.py`。

## 貢獻指南

我們歡迎社群貢獻！無論是修復錯誤、改善文件，還是建議新功能，您的參與都有助於讓這個專案更加完善。如果您對這個研究方向感興趣，歡迎加入我們的開源金融 AI 研究社群 [Tauric Research](https://tauric.ai/)。

## 引用

如果您覺得 _TradingAgents_ 對您有所幫助，請引用我們的研究 :)

```
@misc{xiao2025tradingagentsmultiagentsllmfinancial,
      title={TradingAgents: Multi-Agents LLM Financial Trading Framework},
      author={Yijia Xiao and Edward Sun and Di Luo and Wei Wang},
      year={2025},
      eprint={2412.20138},
      archivePrefix={arXiv},
      primaryClass={q-fin.TR},
      url={https://arxiv.org/abs/2412.20138},
}
```
