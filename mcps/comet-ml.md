# Comet ML MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/comet-ml)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage machine learning experiments via Comet — track model metrics, audit project workspaces, and inspect ML run parameters directly from any AI agent.

## Description
Connect your **Comet ML** account to any AI agent and take full control of your machine learning lifecycle through natural conversation.

### What you can do

- **Experiment Tracking** — List and audit machine learning runs to inspect performance metadata, tags, and live execution statuses
- **Numeric Metric Auditing** — Retrieve high-precision numeric endpoints mapping metrics generated dynamically during your training loops
- **Parameter Inspection** — Extract explicit ML properties like learning rates and configurations logged to specific experiment keys
- **Project & Workspace Navigation** — Navigate through organizational namespaces and identify exactly where your ML research resides
- **Run Metadata Analysis** — Discovered disconnected physical limits parsing explicit run structures, timing, and structural configurations

### How it works

1. Subscribe to this server
2. Enter your Comet ML API Key (found in Account Settings > API Keys)
3. Start auditing your ML experiments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists** — track and compare model metrics across experiments without leaving the research flow
- **ML Engineers** — audit experiment parameters and verify training configurations using natural language
- **AI Researchers** — navigate through multiple workspaces and projects to organize complex ML trials
- **MLOps Teams** — monitor active model evaluations and verify experiment completion statuses in real-time


## Available Tools (6)
- **list_workspaces**: Identify bounded routing spaces inside the Headless Comet ML limits
- **list_projects**: Perform structural extraction matching target Projects inside Comet
- **list_experiments**: Discover explicit routing arrays structuring specific logged experiment limits
- **get_experiment**: Retrieve explicit Cloud logging tracing explicit Payload IDs
- **get_experiment_metrics**: Execute static mapping targeting exactly defined numeric bounds natively
- **get_experiment_params**: Inspect internal properties detailing API taxonomy types


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Comet ML** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all projects in workspace 'research-team'"

**🤖 AI Agent:**
> I found 4 projects in 'research-team': 'NLP-LLM-v2', 'Computer-Vision-Edge', 'Tabular-AutoML', and 'Staging-Tests'. Which one would you like to explore?

---

**👤 You:**
> "Get current metrics for experiment 'exp_abc123'"

**🤖 AI Agent:**
> Retrieving metrics for 'exp_abc123'... Current Accuracy: 0.945, Loss: 0.12, Epoch: 45. The run is still active and performance is trending upwards.

---

**👤 You:**
> "What hyperparameters were used in experiment 'exp_789'?"

**🤖 AI Agent:**
> Experiment 'exp_789' used: learning_rate: 0.001, batch_size: 32, optimizer: 'adam', and model_architecture: 'resnet50'. I have the full list of params if you need them.


## ❓ FAQ

**Q: Can my agent retrieve real-time metrics from an active ML run?**
Yes. Use the 'get_experiment_metrics' tool with the experiment key. The agent will pull the latest numeric logged endpoints, allowing you to monitor loss, accuracy, and other custom metrics as they are generated.

**Q: How do I audit the parameters used in a specific experiment?**
Provide the experiment key to your agent. The 'get_experiment_params' tool extracts all logged ML properties, helping you verify hyperparameters like learning rates, batch sizes, and model architectures.

**Q: Can I see a list of all experiments within a specific project?**
Absolutely. Use the 'list_experiments' tool with the project ID. Your agent will surface all ML runs within that project, including their status and metadata, so you can quickly identify the results you need.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/comet-ml](https://vinkius.com/mcp/comet-ml)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Comet ML** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `comet-ml` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Comet ML** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "comet-ml": {
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
