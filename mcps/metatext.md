# Metatext MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/metatext)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

No-code NLP and AI model management via Metatext — run inference and manage datasets.

## Description
Connect your **Metatext** account to any AI agent and take full control of your NLP models and data pipelines through natural conversation.

### What you can do

- **Model Orchestration** — List all trained NLP models and fetch detailed metadata and training statuses
- **Real-time Inference** — Programmatically run predictions, classifications, and extractions using your deployed models
- **Dataset Management** — Enumerate datasets and create new records for model training or evaluation
- **Deployment Monitoring** — List active model deployments and retrieve account usage information
- **Search & Discovery** — Search for specific NLP models by name to quickly access their capabilities

### How it works

1. Subscribe to this server
2. Enter your Metatext API Key
3. Start managing your NLP workflows from Claude, Cursor, or any MCP-compatible client


## Available Tools (10)
- **create_dataset_record**: Create a new record in a dataset
- **get_account_info**: Get account information
- **get_dataset_details**: Get details for a specific dataset
- **get_model_details**: Get details for a specific model
- **list_nlp_datasets**: List all datasets
- **list_model_deployments**: List active model deployments
- **list_nlp_models**: List all trained NLP models
- **list_dataset_records**: List records in a dataset
- **run_model_inference**: Run prediction on a model
- **search_nlp_models**: Search models by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Metatext** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my trained NLP models in Metatext."

**🤖 AI Agent:**
> Retrieving models... I found several models including 'Sentiment Classifier' and 'Entity Extractor'.

---

**👤 You:**
> "Analyze this text with model ID 'mod_123': 'I love this product!'"

**🤖 AI Agent:**
> Running inference... The model predicts 'Positive' with a confidence score of 98.5%.

---

**👤 You:**
> "Add a new record to dataset 'ds_987' with text 'Refund requested' and label 'Support'."

**🤖 AI Agent:**
> Creating record... The entry has been successfully added to dataset 'ds_987'.


## ❓ FAQ

**Q: How do I find my Metatext API Key?**
Log in to Metatext and navigate to your account settings to find and copy your API Key.

**Q: Can I run inference on any model type?**
Yes, as long as the model is fully trained and deployed, you can use the `run_model_inference` tool.

**Q: Is my AI data secure?**
Absolutely. Your token is encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/metatext](https://vinkius.com/mcp/metatext)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Metatext** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `metatext` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Metatext** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "metatext": {
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
