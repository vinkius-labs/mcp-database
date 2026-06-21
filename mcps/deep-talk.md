# Deep Talk MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deep-talk)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/deep-talk-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/deep-talk-mcp)
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


## Available Tools
- **create_batch_prediction**: Requires the dataset ID, pipeline name, and the column containing the text to analyze.

Start a batch prediction job on a dataset
- **get_batch_prediction**: Get the status and results of a specific batch prediction
- **get_pipeline_details**: Get configuration details for a specific pipeline
- **list_batch_predictions**: List all batch prediction jobs and their statuses
- **list_pipelines**: List all NLP analysis pipelines in your Deep Talk account


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


## Installation & Usage

To install and use the **Deep Talk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deep-talk](https://vinkius.com/mcp/deep-talk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
