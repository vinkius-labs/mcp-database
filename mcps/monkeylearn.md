# MonkeyLearn MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/monkeylearn)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/monkeylearn-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/monkeylearn-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Analyze and extract data from text via MonkeyLearn — sentiment analysis and keyword extraction directly from your AI agent.

## Description
Connect your **MonkeyLearn** account to your AI agent and leverage powerful NLP models for text analysis and data extraction through natural conversation.

### What you can do

- **Text Classification** — Use pre-trained or custom classifiers for sentiment analysis, topic detection, and intent classification.
- **Data Extraction** — Automatically pull keywords, entities, and specific data points from raw text strings.
- **Model Discovery** — List and inspect all classifiers, extractors, and pipelines available in your account.
- **Workflow Tracking** — Monitor your automated workflows and processing activity in real-time.
- **Tag Hierarchy** — Access the tag trees used by your models to understand classification structures.
- **Deep Inspection** — Fetch detailed configuration and metadata for specific models using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your MonkeyLearn API Key
3. Start analyzing text from Claude, Cursor, or any MCP client

### Who is this for?

- **Data Scientists** — quickly test NLP models on sample text without writing boilerplate code.
- **Product Managers** — analyze customer feedback or reviews for sentiment and common themes in real-time.
- **Content Teams** — automate keyword extraction for SEO and tagging directly from the editor.


## Available Tools
- **classify_text**: Classify text using a model
- **extract_text**: Extract data from text
- **get_classifier_details**: Get classifier metadata
- **get_extractor_details**: Get extractor metadata
- **list_activity**: List account activity
- **list_classifiers**: g., sentiment analysis, topic detection) available in your account.

List available classifiers
- **list_extractors**: g., keyword extraction, entity recognition) available in your account.

List available extractors
- **list_pipelines**: List MonkeyLearn pipelines
- **list_tag_trees**: List available tag trees
- **list_workflows**: List automated workflows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MonkeyLearn** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Classify the sentiment of this review: 'The product exceeded all my expectations, truly amazing!' using model cl_oZ9GRg8P."

**🤖 AI Agent:**
> I've analyzed the text. The classifier cl_oZ9GRg8P identified the sentiment as 'Positive' with a confidence score of 98.5%.

---

**👤 You:**
> "List all classifiers available in my account."

**🤖 AI Agent:**
> Retrieving your classifiers... I found 4 models: 'Sentiment Analysis' (cl_oZ9GRg8P), 'Topic Detection' (cl_piuz8L9), 'Support Ticket Classifier', and 'Email Intent'. Would you like to check the details for any of these?

---

**👤 You:**
> "Show me my recent processing activity."

**🤖 AI Agent:**
> I've fetched your account activity. In the last 24 hours, you've made 156 API calls across 3 different models, mostly using the 'Sentiment Analysis' classifier. You have plenty of credits remaining for the current period.


## Installation & Usage

To install and use the **MonkeyLearn** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/monkeylearn](https://vinkius.com/mcp/monkeylearn)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
