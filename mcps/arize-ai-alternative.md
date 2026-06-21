# Arize AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/arize-ai-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Monitor ML model performance, detect data drift, and troubleshoot prediction quality with real-time observability dashboards.

## Description
Connect your **Arize AI** account to any AI agent and take full control of your machine learning observability and automated model monitoring workflows through natural conversation.

### What you can do

- **Project & Trace Orchestration** — List and monitor active ML tracing projects programmatically, retrieving detailed high-fidelity execution spans and telemetry data in real-time
- **Dataset Lifecycle Management** — Programmatically create and manage datasets for model evaluation and validation to maintain a perfectly coordinated ML infrastructure
- **Experiment Monitoring** — Access and track ML experiments to understand high-fidelity model performance, drift, and data quality across different environments
- **Model Intelligence Discovery** — Retrieve detailed metadata for specific ML models to coordinate your organizational AI strategy directly through your agent
- **Operational Monitoring** — Access account-level settings and verify API connectivity directly through your agent for instant performance reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Arize dashboard (Settings > API)
3. Start orchestrating your ML observability pipeline from Claude, Cursor, or any MCP client

No more manual logging into observability portals to check model drift or trace spans. Your AI acts as your dedicated ML engineer and observability coordinator.

### Who is this for?

- **ML Engineers** — instantly retrieve span details and analyze model traces using natural language commands
- **Data Scientists** — monitor experiment results and manage datasets for validation without leaving your creative workspace
- **AI Developers** — automate the oversight of LLM and ML model health through simple AI queries


## Available Tools
- **create_dataset**: Create a dataset
- **get_model**: Get model details
- **list_datasets**: List datasets
- **list_experiments**: List experiments
- **list_projects**: List projects
- **list_spans**: List spans


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Arize AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active ML projects in my Arize account."

**🤖 AI Agent:**
> I've retrieved your tracing projects. You currently have 3 active projects, including 'Production Classifier' (ID: 1024) and 'Beta Recommender'. Which one would you like to inspect for recent traces?

---

**👤 You:**
> "Show the recent execution spans for project '1024'."

**🤖 AI Agent:**
> Accessing telemetry data... I found 5 recent spans for project 1024. Most executions are showing low latency (avg 120ms). One span is flagged with a 'Schema Mismatch' warning. Shall I retrieve the detailed metadata for that trace?

---

**👤 You:**
> "Create a new dataset 'Q2_Eval_Data' for model evaluation."

**🤖 AI Agent:**
> Dataset orchestrated! I've successfully created 'Q2_Eval_Data' in your Arize environment. The dataset ID is 'ds_456'. You can now begin uploading model versions for automated high-fidelity validation. Shall I list your available models?


## ❓ FAQ

**Q: How do I find my Arize API Key?**
Log in to your account, navigate to **Settings** > **API**, and generate or copy your unique secret key.

**Q: Can I track model drift via AI?**
Yes! Use the `list_experiments` tool to retrieve data on active model evaluations and track performance variations programmatically.

**Q: How do I retrieve telemetry traces?**
Use the `list_spans` tool to retrieve high-fidelity execution spans and traces for your ML projects directly from the platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arize-ai-alternative](https://vinkius.com/mcp/arize-ai-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Arize AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `arize-ai-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Arize AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "arize-ai-alternative": {
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
