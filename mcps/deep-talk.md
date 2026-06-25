# Deep Talk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deep-talk)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Equip your AI agent to analyze conversation datasets, extract topics, and monitor sentiment via the Deep Talk API.

## Description
Integrate **Deep Talk**, the powerful conversation analysis platform, directly into your AI workflow. Process large-scale conversation data from sources like Intercom or Zendesk, extract key topics and clusters, and analyze sentiment trends using natural language.

### What you can do

- **Dataset Oversight** — List and retrieve metadata for all your uploaded conversation datasets and their processing status.
- **Topic Extraction** — Identify key themes and extracted topics from your conversation data automatically.
- **Sentiment Analytics** — Retrieve summaries of sentiment across your entire customer interaction database.
- **Conversation Clustering** — List clusters of similar conversations identified by Deep Talk's NLP models.

### How it works

1. Connect the Deep Talk integration to your AI assistant.
2. Authorize using your Deep Talk API Key (found in your account settings).
3. Gain deep insights into your customer conversations through intuitive interaction.

### Who is this for?

- **Customer Experience Managers** — Quickly identify common customer pain points and trending topics on the go.
- **Data Analysts** — Retrieve structured conversation clusters and sentiment data for research via chat.
- **Product Teams** — Monitor feedback themes from support channels to inform roadmap planning.


## Available Tools (5)
- **get_pipeline_details**: Get configuration details for a specific pipeline
- **list_batch_predictions**: List all batch prediction jobs and their statuses
- **list_pipelines**: List all NLP analysis pipelines in your Deep Talk account
- **create_batch_prediction**: Requires the dataset ID, pipeline name, and the column containing the text to analyze.

Start a batch prediction job on a dataset
- **get_batch_prediction**: Get the status and results of a specific batch prediction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deep Talk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all conversation datasets currently processed."

**🤖 AI Agent:**
> I've found 5 datasets in your account, including 'Zendesk Support Q2' and 'Intercom Feedback June'. Both are 'Completed'. Would you like to see the extracted topics for 'Zendesk Support Q2'?

---

**👤 You:**
> "Show me the top topics identified in the 'Customer Feedback' dataset."

**🤖 AI Agent:**
> In the 'Customer Feedback' dataset, the top 3 topics are: 'Pricing Plans' (45%), 'Feature Requests - Mobile App' (30%), and 'Login Issues' (25%). Should I list the sub-topics for any of these?

---

**👤 You:**
> "What is the sentiment summary for our recent support interactions?"

**🤖 AI Agent:**
> The sentiment analysis for your latest support dataset shows 65% Positive, 20% Neutral, and 15% Negative interactions. Sentiment has improved by 10% compared to last month. Would you like to see the clusters with the most negative sentiment?


## ❓ FAQ

**Q: How do I get a Deep Talk API Key?**
Log in to your Deep Talk account, navigate to the API section in your settings, and you can generate or retrieve your unique API Key from there.

**Q: Can the agent process real-time conversations?**
This integration currently focuses on analyzing datasets that have already been uploaded and processed within Deep Talk. Real-time streaming analysis is managed via the Deep Talk dashboard or webhook integrations.

**Q: What languages are supported for analysis?**
Deep Talk supports multiple languages for NLP analysis, including English, Spanish, Portuguese, and French. The agent retrieves results based on the analysis performed in your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deep-talk](https://vinkius.com/mcp/deep-talk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deep Talk** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `deep-talk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deep Talk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deep-talk": {
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
