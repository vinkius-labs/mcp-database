# MonkeyLearn MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/monkeylearn-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/monkeylearn-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/monkeylearn-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Analyze text data with custom machine learning models that classify sentiment, extract keywords, and tag topics automatically.

## Description
Connect your **MonkeyLearn** account to any AI agent and run NLP text analysis through natural conversation.

### What you can do

- **Text Classification** — Classify text by sentiment, topic, intent, or custom labels
- **Entity Extraction** — Pull structured data like names, keywords, and addresses from text
- **NLP Workflows** — Run multi-step Studio workflows for complex pipelines
- **Model Management** — List classifiers, extractors, model versions, and tags
- **Account Status** — Verify API connectivity

### How it works

1. Subscribe to this server
2. Enter your MonkeyLearn API Key
3. Start analyzing text from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists** — run NLP models without writing code
- **Product Teams** — classify user feedback and support tickets
- **Marketers** — extract insights from survey responses and reviews


## Available Tools
- **classify_text**: Classify text data
- **extract_text_entities**: Extract entities
- **get_api_status**: Get account status
- **get_classifier_details**: Get classifier info
- **get_extractor_details**: Get extractor info
- **list_classifier_tags**: List model tags
- **list_classifiers**: List text classifiers
- **list_extractor_tags**: List extractor tags
- **list_extractors**: List text extractors
- **list_model_versions**: List model versions
- **list_nlp_workflows**: List account workflows
- **run_workflow**: Run NLP workflow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MonkeyLearn** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Classify this customer review: 'The product is amazing but delivery was slow.'"

**🤖 AI Agent:**
> Classification (Classifier: cl_pi3C7nuL): Tag: 'Mixed' (Confidence: 0.82). Sub-tags: 'Product Quality' → Positive (0.95), 'Delivery' → Negative (0.88). Full text analyzed successfully.

---

**👤 You:**
> "Extract entities from: 'John Smith from Apple Inc. visited our NYC office on March 15.'"

**🤖 AI Agent:**
> Extraction (Extractor: ex_YCya9nrn): Person: 'John Smith' (Confidence: 0.97). Organization: 'Apple Inc.' (0.95). Location: 'NYC' (0.92). Date: 'March 15' (0.99). Total entities found: 4.

---

**👤 You:**
> "List all my classifiers and extractors."

**🤖 AI Agent:**
> Classifiers: 3. 1) 'Sentiment' (cl_pi3C7nuL, Custom, 500 samples). 2) 'Topic Detection' (cl_abc123, Pre-built). 3) 'Intent' (cl_xyz789, Custom, 1200 samples). Extractors: 2. 1) 'Entity Extractor' (ex_YCya9nrn, Pre-built). 2) 'Keyword Extractor' (ex_def456, Custom). Workflows: 1.


## Installation & Usage

To install and use the **MonkeyLearn** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/monkeylearn-alternative](https://vinkius.com/mcp/monkeylearn-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
