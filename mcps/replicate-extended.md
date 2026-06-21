# Replicate MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/replicate-extended)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate machine learning workflows via Replicate — run models, manage predictions, and search for AI assets directly from any AI agent.

## Description
Connect your **Replicate** account to any AI agent to run powerful machine learning models through simple commands.

### What you can do

- **Run Predictions** — Execute any model version with custom inputs and handle webhooks for completion
- **Model Discovery** — Search for public models or list specific versions and their OpenAPI schemas
- **Management** — Create, update, and manage your own models and hardware configurations
- **Monitoring** — Track prediction status, logs, and outputs in real-time
- **Deployment** — Manage deployments and training sessions for custom fine-tuned models

### How it works

1. Subscribe to this server
2. Enter your Replicate API Token
3. Start generating images, text, or audio from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Engineers** — quickly test model versions and inputs without writing boilerplate code
- **Creative Technologists** — generate media assets directly within their workflow
- **Data Scientists** — monitor training jobs and prediction outputs from a unified interface


## Available Tools
- **cancel_prediction**: Cancel a running prediction
- **create_deployment_prediction**: Create a prediction using a dedicated deployment
- **create_deployment**: Create a new private deployment with custom autoscaling
- **create_model**: Create a new model on Replicate
- **create_prediction**: Create a new prediction to run a model
- **create_training**: Create a training to fine-tune an existing model
- **delete_model_version**: Delete a specific model version
- **get_account**: Get details about the authenticated user or organization
- **get_collection**: Get details of a specific model collection
- **get_model**: Get details of a specific model
- **get_model_version**: Get details of a specific model version, including its OpenAPI schema
- **get_prediction**: Get the status and output of a prediction
- **get_training**: Get the status of a training
- **get_webhook_secret**: Get the default webhook secret key for verifying signatures
- **list_collections**: List curated collections of models
- **list_hardware**: List available hardware SKUs and their descriptions
- **list_model_versions**: List all versions of a model
- **list_predictions**: List recent predictions
- **search_models**: Search for public models on Replicate
- **update_model**: Update metadata for an existing model


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Replicate** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for public models related to 'Stable Diffusion' on Replicate."

**🤖 AI Agent:**
> I found several models. The most popular is 'stability-ai/stable-diffusion' (Version: 328bd9...). Would you like to see the input schema for this model?

---

**👤 You:**
> "Run a prediction for model version 5c51d4... with the prompt 'A futuristic city'."

**🤖 AI Agent:**
> Prediction created (ID: pred_123abc). It is currently 'starting'. I will monitor it for you or you can ask me for the status in a moment.

---

**👤 You:**
> "List my most recent predictions."

**🤖 AI Agent:**
> Fetching your history... You have 3 recent predictions. The latest one (pred_123abc) succeeded and generated an image URL. Would you like to see the results?


## ❓ FAQ

**Q: How can I check if my prediction has finished and see the output?**
Use the `get_prediction` tool with your Prediction ID. It will return the current status (starting, processing, succeeded, or failed) along with the output URLs or data once completed.

**Q: Can I search for specific types of models like 'image-to-text'?**
Yes! Use the `search_models` tool with your query. It will return a list of public models matching your terms, including their owners and descriptions.

**Q: Is it possible to stop a model that is taking too long to run?**
Absolutely. Use the `cancel_prediction` tool with the target Prediction ID to immediately stop the execution and prevent further usage costs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/replicate-extended](https://vinkius.com/mcp/replicate-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Replicate** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `replicate-extended` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Replicate** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "replicate-extended": {
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
