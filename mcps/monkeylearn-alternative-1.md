# MonkeyLearn MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/monkeylearn-alternative-1)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/monkeylearn-alternative-1-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/monkeylearn-alternative-1-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate text analysis via MonkeyLearn — classify sentiment, extract keywords, and run custom NLP pipelines directly from any AI agent.

## Description
Connect **MonkeyLearn** to your AI agent to perform advanced Natural Language Processing (NLP) tasks through simple conversation.

### What you can do

- **Text Classification** — Categorize text into labels like Sentiment, Topic, or Intent using pre-trained or custom classifiers via the `classify_text` tool.
- **Data Extraction** — Automatically pull specific entities, keywords, or names from unstructured text using the `extract_data` tool.
- **Workflow Pipelines** — Chain multiple classification and extraction steps into a single automated process using the `run_pipeline` tool.

### How it works

1. Subscribe to this server
2. Enter your MonkeyLearn API Key
3. Start analyzing text from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly process large volumes of feedback or support tickets without writing scripts.
- **Marketing Teams** — monitor brand sentiment and extract trending topics from social media or reviews.
- **Developers** — integrate NLP capabilities into their workflow without managing complex machine learning infrastructure.


## Available Tools
- **classify_text**: g., Sentiment Analysis, Topic Classification) using a specific MonkeyLearn classifier model.

Classify text into predefined labels
- **extract_data**: Extract specific data from text
- **run_pipeline**: Run a MonkeyLearn pipeline on text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MonkeyLearn** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Classify the sentiment of these reviews using model cl_pi3C7JiL: ['I love this!', 'It was okay', 'Terrible experience']"

**🤖 AI Agent:**
> I've analyzed the reviews. The first is classified as 'Positive' (98% confidence), the second as 'Neutral' (75% confidence), and the third as 'Negative' (99% confidence).

---

**👤 You:**
> "Extract keywords from this text using model ex_y7BPYzNG: 'The new smartphone features a high-resolution OLED screen and 5G connectivity.'"

**🤖 AI Agent:**
> I've extracted the following keywords: 'smartphone', 'high-resolution OLED screen', and '5G connectivity'.

---

**👤 You:**
> "Run the support pipeline p_12345 on this customer email to categorize and extract the order ID."

**🤖 AI Agent:**
> The pipeline has processed the email. Category: 'Shipping Issue'. Extracted Order ID: 'ORD-99283'.


## Installation & Usage

To install and use the **MonkeyLearn** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/monkeylearn-alternative-1](https://vinkius.com/mcp/monkeylearn-alternative-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
