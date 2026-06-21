# Nyckel ML MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nyckel-ml)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nyckel-ml-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nyckel-ml-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Classify data and perform semantic search via Nyckel — track ML functions, samples, and labels directly from your AI agent.

## Description
Connect your **Nyckel** machine learning account to your AI agent and leverage powerful automated classification and semantic search through natural conversation.

### What you can do

- **Automated Classification** — Send text or image URLs to your trained ML functions to get instant predictions and confidence scores.
- **Semantic Search** — Query your search function galleries to find semantically similar samples based on input data.
- **Function Management** — List all ML functions in your account and retrieve detailed configuration and metadata.
- **Training Oversight** — Access the data samples used to train your functions and monitor assigned labels.
- **Sample Annotation** — Upload new training samples and manually assign or update classification labels.
- **Label Discovery** — Retrieve the set of all available labels and categories defined for your ML models.
- **Account Insights** — Access profile and workspace metadata for your authenticated Nyckel account.

### How it works

1. Subscribe to this server
2. Enter your Nyckel Client ID and Client Secret
3. Start processing data with AI from Claude, Cursor, or any MCP client

### Who is this for?

- **AI Developers** — quickly test classification models or search galleries without writing custom integration code.
- **Data Scientists** — monitor training samples and prediction accuracy directly from your workspace.
- **Content Moderators** — automate the classification of user-generated content using custom-trained ML functions.


## Available Tools
- **annotate_ml_sample**: Assign label to a sample
- **create_ml_sample**: Add a training sample
- **delete_ml_function**: Delete an ML function
- **get_ml_function**: Get specific function info
- **get_account_info**: Get current account info
- **invoke_ml_function**: Classify data using a function
- **list_ml_functions**: ) in your account.

List all ML functions
- **list_ml_labels**: List available labels
- **list_ml_samples**: List training samples
- **semantic_search**: Perform semantic search


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nyckel ML** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Classify this text: 'The delivery was very late and the food was cold' using function ID 'func_123'."

**🤖 AI Agent:**
> Invoking ML function func_123... The prediction for your text is 'Negative Sentiment' with a confidence score of 98.45%. Shall I check if there are similar historical samples in your database?

---

**👤 You:**
> "Search my product gallery for an image similar to 'https://example.com/shoe.jpg' using function 'func_search_99'."

**🤖 AI Agent:**
> Executing semantic search... I've found 3 semantically similar samples in your gallery. The top match is 'Running Shoe - Blue' (Confidence: 95.2%). Would you like the metadata for the matching samples?

---

**👤 You:**
> "List all the machine learning functions in my Nyckel account."

**🤖 AI Agent:**
> Retrieving ML functions... You have 4 active functions: 'Sentiment Classifier' (func_123), 'Product Search' (func_search_99), 'Logo Detector', and 'Spam Filter'. Which function would you like to inspect?


## Installation & Usage

To install and use the **Nyckel ML** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nyckel-ml](https://vinkius.com/mcp/nyckel-ml)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
