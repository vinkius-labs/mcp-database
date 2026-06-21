# Weights & Biases MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/weights-biases)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Track experiments, monitor ML runs, and manage artifacts on WandB — the developer platform for AI.

## Description
Connect your **Weights & Biases (WandB)** account to any AI agent and manage your machine learning experiments through natural conversation.

### What you can do

- **Project Management** — List all projects within your WandB entity (user or team) to browse your experiment folders
- **Run Monitoring** — List and track individual experiment runs within a project to monitor real-time activity
- **Deep Run Analysis** — Retrieve full details for any run, including latest accuracies, losses, and hyperparameters
- **Artifact Management** — List versioned datasets, models, and other artifacts to track data lineage and dependencies
- **Sweep Tracking** — Monitor automated hyperparameter search sweeps to see optimization progress
- **Reports & Collaboration** — List saved analysis reports and dashboards to access collaborative documentation

### How it works

1. Subscribe to this server
2. Enter your WandB API Key and optional Base URL
3. Start managing your ML experiments through Claude, Cursor, or any MCP-compatible client

No more manual browsing through complex experiment dashboards to check model performance. Your AI agent becomes your ML research assistant.

### Who is this for?

- **Machine Learning Engineers** — monitor model training progress and compare hyperparameters across multiple runs
- **Data Scientists** — track data lineage and manage versioned artifacts for reproducible research
- **Research Teams** — collaborate on experiment reports and monitor shared project sweeps through chat
- **AI Developers** — quickly surface model metrics and experiment summaries for faster development cycles


## Available Tools
- **get_run_details**: Retrieves full details for a specific W&B run, including summary metrics and config
- **list_project_artifacts**: Lists all artifacts (datasets, models, etc.) in a project
- **list_wandb_projects**: Lists all projects within a Weights & Biases entity (user or team)
- **list_project_reports**: Lists all saved analysis reports in a project
- **list_project_runs**: Lists all experiment runs within a specific W&B project
- **list_project_sweeps**: Lists hyperparameter search sweeps within a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weights & Biases** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all runs in my 'transformer-nmt' project for entity 'ai-team'."

**🤖 AI Agent:**
> I found 5 runs in 'transformer-nmt': 'vibrant-sweep-1' (Running), 'crispy-forest-12' (Finished), 'solar-wind-15' (Crashed), and 2 others. Would you like the detailed summary for any of these?

---

**👤 You:**
> "Get the final accuracy and config for run ID 'vibrant-sweep-1'."

**🤖 AI Agent:**
> Run 'vibrant-sweep-1' summary: accuracy = 0.942, loss = 0.156. Config: learning_rate = 0.001, batch_size = 32, optimizer = 'adam'. It finished 2 hours ago after 50 epochs.

---

**👤 You:**
> "What artifacts are available in the 'resnet-training' project?"

**🤖 AI Agent:**
> In project 'resnet-training', I found: 1. 'imagenet-subset' (Dataset, v3), 2. 'resnet50-weights' (Model, v5), and 3. 'training-logs' (Artifact, v1). Would you like to see the versions or metadata for these?


## ❓ FAQ

**Q: Can I check the latest metrics for a specific ML run?**
Yes. Using the `get_run_details` tool, your AI agent can pull the latest logged metrics (like accuracy or loss) and hyperparameters for any specific run ID within your projects.

**Q: Is it possible to list versioned datasets and models?**
Absolutely. The `list_project_artifacts` tool allows you to see all artifacts, including datasets and models, helping you track data lineage and versioning directly through conversation.

**Q: Can I monitor hyperparameter search sweeps via chat?**
Yes. Use the `list_project_sweeps` tool to monitor automated optimization tasks. Your agent will return a list of sweeps in the project so you can track progress without leaving your workspace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/weights-biases](https://vinkius.com/mcp/weights-biases)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Weights & Biases** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `weights-biases` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Weights & Biases** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "weights-biases": {
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
