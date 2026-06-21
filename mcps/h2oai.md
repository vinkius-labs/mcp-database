# H2O.ai MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/h2oai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Manage AI models via H2O.ai — track data frames, monitor machine learning models and training jobs, and audit cloud cluster status directly from any AI agent.

## Description
Connect your **H2O.ai** instance to any AI agent and take full control of your machine learning lifecycle, automated data processing, and cluster monitoring through natural conversation.

### What you can do

- **Data Frame Orchestration** — List structured datasets securely loaded into H2O clusters and retrieve specific dimensional data mapping explicit frame columns natively
- **Model Inventory Auditing** — Iterate through tracked machine learning models previously generated inside your cloud instance to verify performance metrics and versions
- **Inference Monitoring** — Access detailed configuration blocks for active model architectures to verify deployment boundaries and parameters synchronously
- **Training Job Oversight** — Query timeline nodes tracking long-running tasks and model training jobs queued on the cluster to monitor execution progress
- **Cloud Cluster Auditing** — Ping root endpoints defining hardware architecture health and memory utilization within your H2O instances flawlessly
- **MLOps Command Center** — Verify available frames and models to orchestrate complex data science workflows and model evaluations using natural language
- **Status Verification** — Identify precise executing statuses of ongoing jobs to ensure your AI pipeline is operational and within resource limits securely

### How it works

1. Subscribe to this server
2. Enter your H2O.ai Base URL (found in your H2O cluster settings or cloud dashboard)
3. Start managing your machine learning models from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists** — monitor model training jobs and verify frame data without manual cluster dashboard checks
- **ML Engineers** — audit model architectures and track deployment statuses using natural language conversation
- **Product Teams** — verify available AI models and monitor cluster health in real-time
- **Developers** — test and debug H2O.ai integrations and verify data schemas through the chat interface


## Available Tools
- **list_frames**: List frames
- **get_frame**: Get frame
- **list_models**: List models
- **get_model**: Get model
- **list_jobs**: List jobs
- **cloud_status**: Get cloud status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **H2O.ai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all machine learning models in my H2O cluster"

**🤖 AI Agent:**
> Retrieving models... I found 5 models including 'GBM_model_1', 'DeepLearning_v2', and 'AutoML_leader'. Would you like the detailed performance metrics for the AutoML leader model?

---

**👤 You:**
> "What is the current status of the H2O cloud cluster?"

**🤖 AI Agent:**
> Checking cloud status... Your H2O cluster is 'Healthy' with 4 active nodes. Memory usage is at 35% (14GB used out of 40GB total). All hardware architecture endpoints are operational.

---

**👤 You:**
> "Show me the last 3 training jobs"

**🤖 AI Agent:**
> Retrieving jobs... I found 3 recent tasks: 1. GBM Training (Completed, 10m ago). 2. XGBoost Grid Search (Running, 45% complete). 3. Data Parsing (Completed, 1h ago). I can provide more details for any of these jobs.


## ❓ FAQ

**Q: Can my agent list all data frames currently loaded in my H2O cluster?**
Yes. Use the 'list_frames' tool. The agent retrieves the list of structured datasets securely loaded into memory, including their IDs and basic metadata, allowing you to browse available data flawlessly.

**Q: How do I check the progress of a model training job via chat?**
Use the 'list_jobs' tool. Your agent will query the timeline nodes tracking all long-running tasks on the cluster, providing you with the current execution status and progress percentages synchronously.

**Q: Can I see the internal architecture and metrics of a model through the agent?**
Absolutely. Use the 'get_model' tool with the specific model ID. The agent will fetch the detailed configuration blocks, exposing hyperparameters and performance metrics natively within your chat context.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/h2oai](https://vinkius.com/mcp/h2oai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **H2O.ai** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `h2oai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **H2O.ai** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "h2oai": {
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
