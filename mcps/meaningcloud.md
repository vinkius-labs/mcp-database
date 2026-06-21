# MeaningCloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/meaningcloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Advanced text analytics for sentiment analysis, topic extraction, language detection, and automatic summarization.

## Description
Unlock the power of Natural Language Processing with **MeaningCloud**. This server allows your AI agent to perform deep semantic analysis on any text, document, or URL.

### What you can do

- **Sentiment Analysis** — Detect global polarity, irony, and subjectivity in user feedback or articles.
- **Topic Extraction** — Identify people, organizations, places, and abstract concepts automatically.
- **Language Detection** — Recognize the language of a text from over 160 supported options.
- **Text Categorization** — Classify content into industry-standard taxonomies like IAB or Business models.
- **Automatic Summarization** — Extract the most relevant sentences to create concise summaries of long documents.
- **Document Clustering** — Group collections of texts based on their semantic similarity.

### How it works

1. Subscribe to this server
2. Enter your MeaningCloud License Key (API Key)
3. Start analyzing content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — Automate the processing of large volumes of unstructured text for insights.
- **Content Managers** — Categorize and summarize articles or blog posts instantly.
- **Customer Support Leads** — Monitor sentiment and irony in customer tickets to prioritize responses.


## Available Tools
- **categorize_text**: g., IAB_2.0_en, Business_en).

Assign categories to a text based on a taxonomy
- **cluster_text**: Group a collection of documents into clusters
- **detect_language**: Identify the language of a text
- **analyze_sentiment**: Analyze the sentiment of a text
- **summarize_text**: Extract the most relevant sentences to create a summary
- **extract_topics**: Extract topics, entities, and concepts from text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MeaningCloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the sentiment and check for irony in this text: 'Oh great, another update that breaks everything.'"

**🤖 AI Agent:**
> I've analyzed the text using MeaningCloud. The sentiment is 'Negative' with a high confidence of 'Irony' detected. The subjectivity is high, indicating a personal opinion.

---

**👤 You:**
> "Extract the main topics and organizations mentioned in this article: https://example.com/tech-news"

**🤖 AI Agent:**
> I've processed the URL. I found several entities: 'Apple' (Organization), 'Cupertino' (Location), and 'M3 Chip' (Concept). Would you like more details on any of these?

---

**👤 You:**
> "Summarize the following text into exactly 3 sentences: [Long Text Content]"

**🤖 AI Agent:**
> Here is a 3-sentence summary of the document: 1) The company announced record growth. 2) New markets in Asia contributed to 40% of revenue. 3) Future plans include a focus on sustainable energy.


## ❓ FAQ

**Q: Can the AI detect if a customer is being ironic in their feedback?**
Yes. The `analyze_sentiment` tool identifies not only the polarity (positive/negative) but also the presence of irony and the degree of subjectivity in the text.

**Q: How do I extract specific entities like names or locations from a news article?**
Use the `extract_topics` tool. You can provide a URL or raw text, and it will return a structured list of entities (people, places, organizations) and concepts found.

**Q: Is it possible to summarize a long document into a specific number of sentences?**
Absolutely. The `summarize_text` tool allows you to specify the `sentences` parameter to control the length of the generated summary.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/meaningcloud](https://vinkius.com/mcp/meaningcloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MeaningCloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `meaningcloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MeaningCloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meaningcloud": {
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
