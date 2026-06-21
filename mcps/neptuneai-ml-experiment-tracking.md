# Neptune.ai (ML Experiment Tracking) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/neptuneai-ml-experiment-tracking)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage ML experiments via Neptune.ai — track training runs, monitor metrics, and audit model versions.

## Description
Connect your **Neptune.ai** account to any AI agent and take full control of your machine learning experimentation, model versioning, and training telemetry through natural conversation.

### What you can do

- **Experiment Orchestration** — List all managed ML projects and retrieve detailed metadata configurations tracking active runs and workspace boundaries directly from your agent
- **Run Audit & Search** — Discover specific training runs or historical experiment state checkpoints mapping deep ML parameter sets and performance bounds securely
- **Attribute Inspection** — Extract detailed telemetry capturing the exact variables, accuracy metrics, and loss curves logged during specific execution checkpoints natively
- **Model Registry Management** — List and retrieve trained tracking models promoted and logged explicitly, isolating stable versions from ephemeral experimentation runs
- **Organizational Visibility** — Enumerate accessible workspaces and projects to understand your ML research footprint and documentation distribution natively
- **Credential Audit** — Verify specific user identifies and availability details bound inherently against your active service account token securely
- **Metadata Retrieval** — Deep-dive into specific Project or Run IDs to retrieve precise JSON representations and chronological experimentation insights instantly

### How it works

1. Subscribe to this server
2. Enter your Neptune.ai API Token
3. Start managing your ML experiments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists** — monitor training progress and verify model metrics through natural conversation without manual dashboard navigation
- **ML Engineers** — audit the model registry and verify experiment attributes directly from your workspace terminal
- **AI Researchers** — track production model versions and ensure consistent metadata logging across multiple ML projects efficiently


## Available Tools
- **list_projects**: List accessible Neptune workspaces and projects
- **get_project**: Get specific details for a targeted Neptune ML project
- **search_runs**: Search explicitly tracked ML experimentation runs inside a project
- **get_attributes**: Get parameters mapped within an experiment runtime bounds
- **list_models**: List trained tracking models packaged natively within a project
- **get_user**: Get specific user credentials and availability details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Neptune.ai (ML Experiment Tracking)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all training runs for the 'Customer-Churn' project"

**🤖 AI Agent:**
> I've retrieved the training history for 'Customer-Churn'. Highlights include 'churn-exp-123' (Accuracy: 0.92), 'churn-baseline' (Accuracy: 0.85), and 5 other recent runs. Would you like to see the loss curve for the top-performing run?

---

**👤 You:**
> "Show me the metrics for run ID 'churn-exp-123'"

**🤖 AI Agent:**
> Retrieving attributes for 'churn-exp-123'… The model achieved a final accuracy of 92.4% with a validation loss of 0.15. Learning rate was set to 0.001. No anomalous gradients were detected during the final epochs. Would you like the full JSON of all 45 logged attributes?

---

**👤 You:**
> "List all registered models in project 'Fraud-Detection'"

**🤖 AI Agent:**
> I've identified 3 promoted models in 'Fraud-Detection': 'XGBoost-Classifier-v2', 'RandomForest-Baseline', and 'NeuralNet-Prod-v1'. All models are mapped to production-ready weights. Which one would you like to inspect for version history?


## ❓ FAQ

**Q: Can I see the accuracy metrics for a specific ML run through my agent?**
Yes. Use the `get_attributes` tool with your Project ID and Run ID. Your agent will retrieve the detailed telemetry logged during that execution, including accuracy, loss, and any custom attributes defined in your code.

**Q: How do I check which model versions are currently stable in my registry?**
The `list_models` tool retrieves all packaged ML models within a project. Your agent will expose the promoted model versions, helping you distinguish between experimental runs and stable candidates ready for deployment.

**Q: Can my agent search through hundreds of past ML experimentation runs?**
Absolutely. Use the `search_runs` tool with your Project ID. Your agent will query Neptune's tracking server to identify historical experiment state checkpoints, making it easy to locate specific training results across your entire research timeline.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/neptuneai-ml-experiment-tracking](https://vinkius.com/mcp/neptuneai-ml-experiment-tracking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Neptune.ai (ML Experiment Tracking)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `neptuneai-ml-experiment-tracking` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Neptune.ai (ML Experiment Tracking)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "neptuneai-ml-experiment-tracking": {
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
