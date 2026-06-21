# Abacus AI (Enterprise AI Cloud) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/abacus-ai-enterprise-ai-cloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Manage the full machine learning lifecycle via Abacus AI — create projects, train models, and deploy real-time prediction endpoints.

## Description
Connect your **Abacus AI** enterprise account to any AI agent to orchestrate complex machine learning workflows through natural language. This server provides a direct bridge to the Abacus AI Enterprise Cloud, enabling seamless MLOps from your workspace.

### What you can do

- **Project Orchestration** — List existing machine learning projects or create new ones tailored to specific use cases like retail recommendations or churn prediction.
- **Data Management** — Create and inspect datasets, allowing your agent to understand the underlying data structures and metadata before training.
- **Model Training** — Initiate training jobs for machine learning models directly from a conversation, including custom training configurations.
- **Deployment & Inference** — Deploy trained models to real-time endpoints and retrieve instant predictions using deployment tokens.
- **Status Monitoring** — Query the health and metrics of your models and datasets to ensure your AI infrastructure is performing optimally.

### How it works

1. Subscribe to this server
2. Enter your Abacus AI API Key
3. Start managing your ML models and datasets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists** — quickly check model training status or dataset metadata without switching to the Abacus web console.
- **ML Engineers** — automate the deployment of trained models and test prediction endpoints directly from the terminal or IDE.
- **AI Product Managers** — monitor project progress and verify model metrics through simple natural language queries.


## Available Tools
- **create_project**: Create a new project
- **describe_model**: Returns the status and details of a model
- **train_model**: Starts a training job for a model
- **create_dataset**: Create a new dataset
- **create_deployment**: Deploys a trained model to a real-time endpoint
- **describe_dataset**: Returns metadata about a specific dataset
- **get_prediction**: Retrieves a prediction from a deployed model
- **list_projects**: List all projects in your organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Abacus AI (Enterprise AI Cloud)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my machine learning projects in Abacus AI."

**🤖 AI Agent:**
> I've retrieved your projects. You have 3 active projects: 'Customer Churn' (ID: proj_123), 'Demand Forecast' (ID: proj_456), and 'Lead Scoring' (ID: proj_789).

---

**👤 You:**
> "Start training a model named 'SalesModel_v1' in project proj_123."

**🤖 AI Agent:**
> The training job for 'SalesModel_v1' has been initiated in project proj_123. You can check its progress using the model ID provided: model_abc123.

---

**👤 You:**
> "Get a prediction from deployment dep_999 using this data: {"user_id": "123", "last_purchase": 50}."

**🤖 AI Agent:**
> The model predicts a 'churn_probability' of 0.15 for this user based on the provided data.


## ❓ FAQ

**Q: How can I check if my model training is finished?**
You can use the `describe_model` tool by providing the unique Model ID. It will return the current status, metrics, and other details of the training job.

**Q: Can I get a prediction from a deployed model directly through the agent?**
Yes! Use the `get_prediction` tool. You will need the deployment ID, the deployment token, and the input data in JSON format to receive a real-time prediction.

**Q: Is it possible to create a new project for a specific ML use case?**
Absolutely. Use the `create_project` tool and specify the name and the `useCase` (e.g., 'RETAIL_RECOMMENDATIONS') to initialize a project tailored for that specific application.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/abacus-ai-enterprise-ai-cloud](https://vinkius.com/mcp/abacus-ai-enterprise-ai-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Abacus AI (Enterprise AI Cloud)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `abacus-ai-enterprise-ai-cloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Abacus AI (Enterprise AI Cloud)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "abacus-ai-enterprise-ai-cloud": {
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
