# Conduit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/conduit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Equip your AI agent to observe data streams, manage integration pipelines, and monitor nodes on the Conduit platform.

## Description
Connect your AI agent seamlessly with **Conduit**, the modern data integration and synchronization platform. Utilizing natural language interactions, users can instruct the AI to oversee active streaming health, check connectors, and extract pipeline logs without accessing the conventional web dashboard interfaces.

### What you can do

- **Pipeline Management** — Request status overviews of active, paused, or degraded data integration pipelines efficiently.
- **Connector Auditing** — Ask the agent to locate specific connectors (source or destination) mapped to your critical infrastructure.
- **Log Evaluation** — Fetch recent application logs or streaming output reports via conversation to debug integration errors on the fly.

### How it works

1. Append this integration into your AI application interface securely.
2. Authorize connections providing the target instance Base URL, corresponding API Key, and an active Admin Password if applicable.
3. Chat natively instructing your agent to inspect and orchestrate streams through plain text inputs directly.

### Who is this for?

- **Data Engineers** — Instantly review health metrics regarding continuous synchronization services running between complex databases.
- **DevOps Professionals** — Confirm that new pipeline deployments successfully connected endpoints after infrastructure modifications.
- **System Administrators** — Request aggregate tracking reports validating if crucial operational data streams function continuously overnight.


## Available Tools
- **get_run_status**: Returns detailed status, timing, and error information.

Retrieve the current status of a specific workflow run
- **get_workflow**: Returns source, destination, and current status.

Retrieve detailed information about a specific workflow
- **list_connections**: Retrieve a list of all active source and destination connections
- **list_available_destinations**: Retrieve available data destination connector types supported by Conduit
- **list_workflow_runs**: Returns the execution history with status and timestamps for each run.

Retrieve the history of runs for a specific workflow
- **list_available_sources**: Retrieve available data source connector types supported by Conduit
- **list_workflows**: Use this as a starting point to discover workflow IDs for subsequent operations.

Retrieve a list of all data integration workflows in Conduit
- **trigger_workflow**: Use list_workflows first to find the workflow ID.

Manually trigger a run for a specific workflow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Conduit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve the current status of all major pipelines running in the production Conduit instance."

**🤖 AI Agent:**
> I checked your pipelines successfully. Of the 8 tracked major pipelines running on the queried instance: 7 are currently marked as 'Running' with no latency spikes or recorded disruption alerts. Pipeline ID 'PG_to_Snowflake_04' is however marked 'Degraded' due to a destination connector timeout 4 minutes ago. Do you want further logs related to this degraded element specifically to review the exact recorded error response logged safely here?

---

**👤 You:**
> "Check if there's a configured destination connector named 's3-analytics-bucket' and briefly describe its configuration parameters."

**🤖 AI Agent:**
> Yes, I located the 's3-analytics-bucket' destination connector attached to your integration pipelines successfully. This configured destination strictly utilizes the official 'builtin:s3' plugin structure. The setup parameters authenticate via attached AWS Keys (redacted), targeting an external region of 'us-east-1', and output streams correctly in a structured JSON payload referencing an established logical path.

---

**👤 You:**
> "Pause the pipeline 'MySQL-to-Kafka' immediately."

**🤖 AI Agent:**
> I'm sorry, but for safety reasons, I can only inspect pipelines and display logs. I cannot pause, modify, or delete pipelines. Please use the Conduit dashboard to execute this action.


## ❓ FAQ

**Q: How do I systematically obtain an active API Key targeting the Conduit platform?**
Depending absolutely on how your infrastructure deployed the program (standalone desktop executable, core Docker containerized setups, or external Cloud instance providers), keys are defined at setup. Generally, navigate your hosted interface configurations to visually spot specific 'API section' panels or define standard keys via backend environment base configurations (for Docker setup instances, parameters typically refer natively mapping to 'CONDUIT_API_URL'). Insert keys properly downwards with other core data completely preserving original syntax precisely achieving seamless valid interactive integrations securely effortlessly resolving requirements seamlessly connecting completely natively without technical failures preventing operations running clearly correctly natively actively continuously stably.

**Q: Can the text-based conversational integration construct entirely new data mapping pipelines logically?**
For maintaining stability and avoiding potentially flawed or disruptive integration commands inadvertently given through free text models over critical systems, this integration focuses capabilities mostly on analytical monitoring, status reviewing and component checks (observer and reporting methodologies). Direct architectural construction mapping entire data flow pipelines heavily relies on original detailed configurations inside Conduit visually rather than natural language textual generative guesses mitigating potential serious enterprise data leaks implicitly actively safely limiting functions structurally appropriately maintaining steady uncompromised safe connections.

**Q: Which connector types can the AI list?**
The integration can list both source and destination connectors configured in your Conduit instance. Use the pipeline inspection tools to see which plugins are attached, their configuration parameters, and their current health status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/conduit](https://vinkius.com/mcp/conduit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Conduit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `conduit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Conduit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "conduit": {
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
