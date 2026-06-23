# Modelbit (ML Model Deployments) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/modelbit-ml-model-deployments)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Deploy and call machine learning models directly from your AI agent using Modelbit's inference endpoints.

## Description
Connect your **Modelbit** workspace to any AI agent to run production-grade machine learning models through natural conversation.

### What you can do

- **Model Inference** — Call any deployed ML model (Python, Scikit-learn, PyTorch, etc.) using the `get_inference` tool to get real-time predictions.
- **Version Control** — Specify exact model versions or tags (like 'latest' or 'v2') to ensure consistent and reproducible outputs.
- **Data Integration** — Pass complex JSON objects or arrays directly to your models and receive computed results instantly.
- **Seamless MLOps** — Bridge the gap between your data science notebooks and your AI assistant's reasoning capabilities.

### How it works

1. Subscribe to this server
2. Enter your Modelbit Workspace name
3. (Optional) Enter your Modelbit API Key for private deployments
4. Start getting predictions from your models in Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists** — test and showcase model outputs directly within an AI chat interface
- **ML Engineers** — integrate production models into AI-driven workflows without building custom glue code
- **Product Teams** — prototype AI features that rely on custom proprietary machine learning logic


## Available Tools (1)
- **get_inference**: Use this to pass data to your ML models and receive the computed output.

Call a deployed Modelbit machine learning model


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Modelbit (ML Model Deployments)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Call the 'sales_forecast' model with data: {'region': 'north', 'month': 12}."

**🤖 AI Agent:**
> I've sent the request to the 'sales_forecast' deployment. The model predicts a revenue of $450,000 for the North region in December.

---

**👤 You:**
> "Get an inference from 'image_classifier' version 'v2' for this input array of pixel values."

**🤖 AI Agent:**
> Using version 'v2' of 'image_classifier', the model has identified the object as 'high-resolution satellite imagery' with 98% confidence.

---

**👤 You:**
> "Run the 'fraud_detection' model on the latest transaction data."

**🤖 AI Agent:**
> I've executed the `get_inference` tool for 'fraud_detection'. The model flagged the transaction as 'low risk' (score: 0.02).


## ❓ FAQ

**Q: Can I specify which version of a model to use for inference?**
Yes. When using the `get_inference` tool, you can provide an optional `version` string (e.g., 'v1', 'latest', or a specific tag) to target a precise deployment.

**Q: What format should the input data be in?**
The `get_inference` tool accepts a `data` parameter which should be a JSON object or array, matching the input schema expected by your Modelbit deployment.

**Q: Is an API Key required for all models?**
The `MODELBIT_API_KEY` is optional. It is only required if your Modelbit deployment is private. Public deployments only require the `MODELBIT_WORKSPACE` name.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/modelbit-ml-model-deployments](https://vinkius.com/mcp/modelbit-ml-model-deployments)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Modelbit (ML Model Deployments)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `modelbit-ml-model-deployments` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Modelbit (ML Model Deployments)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "modelbit-ml-model-deployments": {
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
