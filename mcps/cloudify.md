# Cloudify MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloudify)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Orchestrate cloud infrastructure via Cloudify — manage blueprints, deployments, and monitor workflow executions directly from any AI agent.

## Description
Connect your **Cloudify Manager** to any AI agent and take full control of your multi-cloud orchestration through natural conversation.

### What you can do

- **Blueprint Management** — List and audit OASIS TOSCA blueprints parsing root Cloudify manager templates
- **Deployment Tracking** — Retrieve exact structural matching of actualized runtime schemas and manage infrastructure states
- **Workflow Executions** — Monitor install, uninstall, and heal transactions to track deployment events in real-time
- **Node Inspections** — Resolve deeply nested infrastructure nodes and audit lifecycle properties (started, created, deleted)
- **Plugin Auditing** — Discover installed Python abstractions for AWS, GCP, and other cloud integrations

### How it works

1. Subscribe to this server
2. Enter your Cloudify Manager URL and API Token
3. Start orchestrating your infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Cloud Engineers** — manage complex orchestration blueprints and deployments using natural language
- **DevOps Teams** — monitor workflow executions and node states without digging through the manager UI
- **Platform Architects** — audit multi-cloud integrations and plugin configurations across environments
- **SREs** — quickly identify failed executions and verify infrastructure lifecycle states


## Available Tools (7)
- **list_blueprints**: Identify bounded logical arrays managing top-level orchestration schemas
- **get_blueprint**: Perform structural extraction of properties driving active blueprint schemas
- **list_deployments**: Retrieve the exact structural matching verifying actualized runtime schemas
- **get_deployment**: Extracts explicitly attached internal structural states pulling precise execution topologies
- **list_executions**: Identify precise active cluster limits spanning deployment workflow bounds
- **list_nodes**: Identify exact literal limits pushing specific instances routing orchestration rules
- **list_plugins**: Extracts explicit capabilities mapping native orchestration limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cloudify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all blueprints in Cloudify Manager"

**🤖 AI Agent:**
> I found 5 blueprints. The active ones are: 'aws-three-tier', 'gcp-k8s-cluster', and 'hybrid-db-template'. Which one would you like to inspect?

---

**👤 You:**
> "Show me the execution history for deployment 'web-app-prod'"

**🤖 AI Agent:**
> Retrieving executions for 'web-app-prod'... The last workflow was 'install' which finished successfully. There is a 'heal' execution from yesterday that was triggered automatically.

---

**👤 You:**
> "What nodes are currently in the 'started' state for deployment 'db-cluster'?"

**🤖 AI Agent:**
> Analyzing nodes for 'db-cluster'... I found 3 nodes in 'started' state: 'primary-node-1', 'replica-node-1', and 'load-balancer-internal'. All instances are healthy.


## ❓ FAQ

**Q: Can my agent list all active cloud deployments?**
Yes. Use the 'list_deployments' tool. Your agent will retrieve the exact structural matching of your actualized runtime schemas, showing you every environment currently managed by Cloudify.

**Q: How do I check the lifecycle state of a specific infrastructure node?**
Provide the deployment ID to your agent and use the 'list_nodes' tool. The agent will resolve deeply nested nodes and identify whether instances are in 'started', 'created', or 'deleted' states.

**Q: Can I monitor pending workflow executions through the agent?**
Absolutely. The 'list_executions' tool surfaces active mapping for install, uninstall, and heal workflows. This allows you to track transactions and deployment events strictly within Cloudify limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloudify](https://vinkius.com/mcp/cloudify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cloudify** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cloudify` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cloudify** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cloudify": {
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
