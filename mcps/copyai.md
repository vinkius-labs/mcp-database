# Copy.ai MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/copyai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to automate content production and business processes using Copy.ai Workflows.

## Description
Integrate **Copy.ai**, the AI OS for GTM (Go-to-Market), directly into your workflow. Leverage powerful AI Workflows to automate repetitive tasks, generate high-quality content, and scale your operations using natural language.

### What you can do

- **Execute Workflows** — Run any of your pre-defined Copy.ai Workflows with custom inputs via chat.
- **Status Monitoring** — Track the progress and results of active workflow runs in real-time.
- **Asset Management** — Access your Brand Voice and Info Base to ensure consistent content quality.
- **Discovery** — List and search for workflows and folders across your workspace.

### How it works

1. Connect the Copy.ai integration to your AI assistant.
2. Authorize using your Copy.ai API Key (found in Workspace Settings > API Keys).
3. Automate your marketing and sales tasks through intuitive conversation.

### Who is this for?

- **Marketing Teams** — Scale content creation and maintain brand consistency effortlessly.
- **Sales Operations** — Automate lead research and personalized outreach sequences.
- **Content Strategists** — Quickly trigger complex multi-step AI processes via chat.


## Available Tools
- **delete_webhook**: Remove a registered webhook
- **get_workflow_run_status**: Status can be PROCESSING, COMPLETE, or FAILED.

Check the status and results of a workflow run
- **get_webhook**: Get details of a specific webhook
- **list_workflow_runs**: List past executions of a workflow
- **list_webhooks**: ai account.

List all registered webhooks
- **register_webhook**: Register a webhook for workflow events
- **run_workflow**: Provide the workflow ID and starting variables as a JSON object. Returns a run_id to track progress.

Start a Copy.ai workflow execution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Copy.ai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all content automation workflows in my workspace."

**🤖 AI Agent:**
> I found 5 content automation workflows, including 'SEO Blog Generator' and 'Social Media Post Multiplier'. Which one would you like to run?

---

**👤 You:**
> "Run the 'Lead Researcher' workflow for the domain 'vinkius.com'."

**🤖 AI Agent:**
> Workflow 'Lead Researcher' started for 'vinkius.com' (Run ID: r8s9df). I'll let you know once the research is complete. Should I summarize the findings here?

---

**👤 You:**
> "Check the status of my latest workflow run."

**🤖 AI Agent:**
> Your latest run (ID: r8s9df) is 100% complete. It successfully analyzed 'vinkius.com' and identified 12 key decision-makers. Would you like to see the list?


## ❓ FAQ

**Q: How do I get a Copy.ai API Key?**
Log in to your Copy.ai workspace, go to **Settings > API Keys**, and click 'Create API Key'. Copy the generated secret key and paste it below.

**Q: What are Workflows in Copy.ai?**
Workflows are multi-step AI processes that can automate complex tasks like lead research, content generation, and data enrichment. This integration allows you to trigger them directly from chat.

**Q: Can the agent access my Brand Voice?**
Yes, if your workflow is configured to use your Brand Voice or Info Base, the agent can trigger those processes ensuring the output aligns with your brand standards.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/copyai](https://vinkius.com/mcp/copyai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Copy.ai** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `copyai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Copy.ai** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "copyai": {
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
