# n8n (AI Workflow Automation) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/n8n-ai-workflow-automation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage workflow automation via n8n — audit active workflows, track execution logs, and monitor credentials.

## Description
Connect your **n8n** instance to any AI agent and take full control of your node-based workflow automation, execution diagnostics, and project orchestration through natural conversation.

### What you can do

- **Workflow Orchestration** — List all managed automation workflows and retrieve detailed JSON logic nodes, including link mappings and trigger configurations directly from your agent
- **Execution Diagnostics** — Extract historical execution logs to track success/failure boundaries and retrieve absolute trace logs for rapid debugging of automation failures
- **Node-Level Inspection** — Deep-dive into specific execution IDs to extract bounded node-level output blocks and identify exact processing errors natively
- **Credential Audit** — List metadata mapping saved automation credentials to verify system types and IDs without exposing literal secure tokens
- **Collaborative Visibility** — Enumerate provisioned team users and assigned roles to verify access targets across your n8n infrastructure securely
- **Organizational Tags** — List arbitrary category tags used to group and sort complex workflow logic dimensions across your automation workspace
- **Metadata Inspection** — Retrieve precise graph representations for specific workflows to understand the underlying logic and data transformation flows instantly

### How it works

1. Subscribe to this server
2. Enter your n8n Base URL and API Key
3. Start managing your automation node from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Automation Engineers** — verify workflow designs and debug execution failures through natural conversation without manual dashboard navigation
- **Software Developers** — test node-based automation logic and retrieve execution traces directly from your workspace terminal
- **IT Operations Teams** — monitor automation health and audit credential mappings across multiple n8n instances efficiently


## Available Tools (7)
- **list_instance_users**: List collaborators on the n8n instance
- **list_workflows**: List n8n automation workflows
- **list_stored_credentials**: List metadata for saved credentials
- **list_workflow_executions**: List recent workflow executions
- **get_execution_details**: Get trace logs for a specific execution
- **get_workflow_details**: Get details for a specific workflow
- **list_workflow_tags**: List workflow organizational tags


## 💬 Prompt Examples

Here are some examples of how you can interact with the **n8n (AI Workflow Automation)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active workflows in my n8n instance"

**🤖 AI Agent:**
> I've retrieved your n8n workflows. Highlights include 'Shopify-to-Slack-Sync' (ID: 12, Active), 'Customer-Onboarding-Email' (ID: 45, Active), and 'Daily-Database-Cleanup' (ID: 78). Would you like to check the last execution status for any of these?

---

**👤 You:**
> "Show me the last 5 failed executions in n8n"

**🤖 AI Agent:**
> Retrieving failed executions… I've identified 5 recent errors. The most recent failure was in workflow 'Lead-Ingestion' (ID: 135) due to an 'Unauthorized' error on the CRM node. Would you like me to fetch the full trace for that execution?

---

**👤 You:**
> "List all n8n credentials associated with 'Slack'"

**🤖 AI Agent:**
> I've identified 2 credentials matching 'Slack': 1) 'Slack-Main-Workspace' (ID: 5, Type: slackApi), and 2) 'Slack-Support-Bot' (ID: 8, Type: slackApi). Both appear to be valid. Would you like to check the tags associated with these workflows?


## ❓ FAQ

**Q: Does this work with self-hosted n8n instances?**
Yes. You just need to provide your full n8n Base URL (e.g., https://n8n.your-company.com). Your agent will connect securely to your private instance using your n8n API Key.

**Q: Can I see exactly why an n8n execution failed through my agent?**
Yes. Use the `get_execution` tool with a specific Execution ID. Your agent will retrieve the node-level trace logs, allowing you to see which specific node encountered an error and the resulting output payload for that step.

**Q: Can my agent list the automation credentials saved in my n8n account?**
Absolutely. Use the `list_credentials` tool to identify all stored auth hooks. Your agent will report the credential names and system types (e.g., Slack, GitHub), helping you audit your integrations without exposing literal secure tokens.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/n8n-ai-workflow-automation](https://vinkius.com/mcp/n8n-ai-workflow-automation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **n8n (AI Workflow Automation)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `n8n-ai-workflow-automation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **n8n (AI Workflow Automation)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "n8n-ai-workflow-automation": {
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
