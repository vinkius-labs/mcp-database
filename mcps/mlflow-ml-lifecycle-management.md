# MLflow (ML Lifecycle Management) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mlflow-ml-lifecycle-management)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Manage ML lifecycle via MLflow — track training runs, monitor metrics, and audit the model registry.

## Description
Connect your **MLflow** tracking server to any AI agent and take full control of your machine learning experiments, training telemetry, and model registry through natural conversation.

### What you can do

- **Run Orchestration** — Search and retrieve detailed Model Training Runs across specific experiments to track accuracy metrics, loss curves, and scalar parameters directly from your agent
- **Experiment Audit** — List all registered MLflow experiments and retrieve detailed metadata configurations to understand how your project's research branches are structured
- **Metric Inspection** — Extract explicit telemetry capturing the exact state vectors and performance metrics logged during atomic training sessions for rapid diagnostic analysis
- **Model Registry Management** — Search the Global Model Registry to identify models explicitly promoted to production or staging pipelines and track version deployments securely
- **Artifact Visibility** — List physical storage boundaries referencing stored model blobs, image graphs, or metadata saved natively inside MLflow training runs
- **Telemetry Mapping** — Aggregate tracking logs from multiple experiments to identify trends and compare model performance across different historical training sessions

### How it works

1. Subscribe to this server
2. Enter your MLflow Tracking URI and Tracking Token
3. Start managing your ML experiments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists** — monitor training progress and verify model metrics through natural conversation without manual dashboard navigation
- **ML Engineers** — audit the model registry and verify artifact storage locations directly from your workspace terminal
- **AI Operations Teams** — track production model versions and ensure consistent deployment of high-performing ML models efficiently


## Available Tools
- **search_experiments**: Search all MLflow registered Experiments explicitly
- **get_experiment**: Get an explicit explicit MLflow Experiment by ID configuration
- **search_runs**: Search exact Model Training Runs across specific Experiments
- **get_run**: Get parameters and metrics mapping a specific atomic Run ID
- **search_registered_models**: Search the MLflow Global Model Registry
- **list_artifacts**: List static artifacts attached over a specific Run


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MLflow (ML Lifecycle Management)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all training runs for the 'Sentiment Analysis' experiment"

**🤖 AI Agent:**
> Retrieving training history… I've identified 12 runs for 'Sentiment Analysis'. The latest run 'bright-fox-123' achieved 92% accuracy with a 0.12 loss. Other recent runs show similar performance with varying hyperparameters. Would you like to see the parameter logs for the best run?

---

**👤 You:**
> "What models are currently marked as 'Production' in the registry?"

**🤖 AI Agent:**
> Scanning model registry… I've identified 3 models in Production: 'Customer-Churn-Classifier' (v4), 'Product-Recommender-Engine' (v12), and 'Demand-Forecaster' (v2). I can provide the tracking URI or source run ID for any of these production models if you'd like.

---

**👤 You:**
> "Show me the artifacts saved for run ID 'bright-fox-123'"

**🤖 AI Agent:**
> Retrieving artifacts for 'bright-fox-123'… I've identified the following files: 1) 'model.pkl' (Pickled model), 2) 'confusion_matrix.png' (Visualization), 3) 'feature_importance.csv', and 4) 'conda.yaml'. I can provide the source tracking path for these files securely.


## ❓ FAQ

**Q: Can I see the metrics for a specific training run through my agent?**
Yes. Use the `get_run` tool with a specific Run ID. Your agent will retrieve the detailed telemetry logged during that training session, including scalars like accuracy, loss, or any custom performance metrics you've defined.

**Q: How do I check which models are ready for production in the registry?**
The `search_registered_models` tool allows your agent to query the global model registry. You can identify models that have been explicitly promoted to production or staging environments, helping you track deployment states across your project.

**Q: Can my agent list the plots or model files saved in a specific run?**
Absolutely. Use the `list_artifacts` tool with a specific Run ID. Your agent will report all physical storage boundaries, including stored model blobs (e.g., .pkl, .h5) and saved image plots, ensuring you can locate critical training artifacts instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mlflow-ml-lifecycle-management](https://vinkius.com/mcp/mlflow-ml-lifecycle-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MLflow (ML Lifecycle Management)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mlflow-ml-lifecycle-management` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MLflow (ML Lifecycle Management)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mlflow-ml-lifecycle-management": {
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
