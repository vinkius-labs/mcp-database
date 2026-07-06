# NLP Cloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nlp-cloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

High-performance NLP API for text summarization, entity extraction, classification, sentiment analysis, ASR, and translation.

## Description
Integrate **NLP Cloud** into your AI workflows to leverage state-of-the-art Natural Language Processing models. This MCP server allows your agent to process text and audio with professional-grade accuracy.

### Key Features

- **Text Summarization** — Condense long documents into concise summaries using models like BART or GPT.
- **Entity Extraction (NER)** — Automatically identify names, dates, locations, and organizations within any text block.
- **Sentiment & Emotion** — Analyze the tone of customer feedback or social media posts to detect positive/negative sentiment.
- **Zero-Shot Classification** — Categorize text into custom labels without needing specific training data.
- **Speech Recognition (ASR)** — Convert audio and video files into accurate text transcripts using Whisper.
- **Translation** — Translate content between dozens of languages using high-accuracy NLLB models.

### How it works

1. Subscribe to this server
2. Enter your NLP Cloud API Token
3. Start processing advanced NLP tasks from Claude, Cursor, or any MCP client

### Who is this for?

- **Data Scientists & Developers** — Quickly test and integrate NLP capabilities into applications without managing infrastructure.
- **Content Managers** — Automate summarization and tagging of large volumes of articles or reports.
- **Customer Support Leads** — Analyze sentiment and categorize incoming tickets at scale.


## Available Tools (6)
- **classify_text**: Categorize text into predefined labels
- **extract_entities**: Extract named entities (NER) from text
- **analyze_sentiment**: Determine the sentiment of text
- **summarize_text**: Summarize a block of text
- **translate_text**: Provide the required JSON payload as per NLP Cloud docs.

Translate text between languages
- **perform_asr**: Provide the required JSON payload as per NLP Cloud docs.

Extract text from audio or video files (ASR)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NLP Cloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Summarize this text using the bart-large-cnn model: [Insert Text]"

**🤖 AI Agent:**
> I've summarized the text for you. Here is the condensed version: [Summary Content].

---

**👤 You:**
> "Extract all named entities from this paragraph: [Insert Text]"

**🤖 AI Agent:**
> I found the following entities: 'Apple' (Organization), 'Cupertino' (Location), and 'September 12th' (Date).

---

**👤 You:**
> "What is the sentiment of this customer review: 'The product exceeded my expectations!'"

**🤖 AI Agent:**
> The sentiment analysis shows a 'Positive' result with a high confidence score.


## ❓ FAQ

**Q: Can I summarize a long article using a specific model like BART?**
Yes! Use the `summarize_text` tool and specify the `model` (e.g., 'bart-large-cnn') along with your text. You can also enable `use_gpu` for faster processing.

**Q: How do I extract names and locations from a document?**
You can use the `extract_entities` tool. Provide the text and a NER model (like 'en_core_web_lg'), and the agent will return a list of identified entities such as persons, organizations, and locations.

**Q: Is it possible to transcribe audio files into text?**
Absolutely. Use the `perform_asr` tool with a model like 'whisper'. You'll need to provide a JSON payload containing the audio URL or data as required by the NLP Cloud API.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nlp-cloud](https://vinkius.com/mcp/nlp-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NLP Cloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nlp-cloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NLP Cloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nlp-cloud": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
