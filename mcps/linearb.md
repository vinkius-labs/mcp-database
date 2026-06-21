# LinearB MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linearb)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Export software delivery metrics, manage deployments, and report incidents via the LinearB API.

## Description
Connect your **LinearB** account to any AI agent to automate your engineering intelligence and DORA metrics reporting. This MCP server enables your agent to query cycle time, track deployments, and report incidents directly from natural language interfaces.

### What you can do

- **Metric Ingestion** — Query complex engineering metrics including cycle time, coding time, and pickup time across teams
- **Deployment Management** — Inform LinearB of new software releases by reporting Git refs (SHAs or tags) programmatically
- **Incident Tracking** — Report and list engineering incidents to maintain accurate Change Failure Rate and MTTR metrics
- **Metadata Oversight** — List teams and connected repositories to map technical IDs to organizational structures
- **DORA Analytics** — Retrieve aggregated performance data to identify bottlenecks in your delivery pipeline

### How it works

1. Subscribe to this server
2. Enter your LinearB Public API Key
3. Start managing your engineering metrics from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Engineering Managers** — Monitor team cycle times and delivery health via simple natural language commands
- **DevOps Engineers** — Automate the reporting of deployments and incidents directly from CI/CD pipelines or IDEs
- **CTOs** — Quickly audit organizational performance and DORA metrics without opening the dashboard


## Available Tools
- **record_new_deployment**: Requires repo_id and ref.

Report a new deployment to LinearB
- **record_new_incident**: Requires provider_id and started_at.

Report a new incident
- **list_software_deployments**: List recent deployments
- **list_software_incidents**: List engineering incidents
- **query_software_metrics**: Requires a JSON body with requested_metrics and time_ranges.

Query software engineering metrics (v2)
- **list_connected_repos**: List all connected repositories
- **list_engineering_teams**: List all teams defined in LinearB


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LinearB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Query the average cycle_time for the last 30 days for team 'Backend'."

**🤖 AI Agent:**
> I've retrieved the metrics for team 'Backend'. The average cycle_time over the last 30 days is 3.5 days, with coding_time at 1.2 days and pickup_time at 0.8 days.

---

**👤 You:**
> "Record a new deployment for repo ID '123' with Git ref 'v1.2.0'."

**🤖 AI Agent:**
> Successfully informed LinearB of the new deployment. The Git ref 'v1.2.0' for repository 123 has been recorded, and cycle times for the included PRs will be updated.

---

**👤 You:**
> "Report a new incident starting now for provider 'OpsGenie'."

**🤖 AI Agent:**
> I've reported the incident to LinearB. It has been associated with provider 'OpsGenie' starting at [timestamp]. This will be used to calculate your MTTR.


## ❓ FAQ

**Q: How do I query cycle time for a specific team?**
Use the `query_software_metrics` tool and include the team name or ID in the `group_by` parameter of your JSON query.

**Q: What is the difference between coding_time and pickup_time?**
Coding time is the duration from the first commit to the PR creation. Pickup time is the duration from the PR creation to the first review activity.

**Q: Can I report a release from the agent?**
Absolutely. Use the `record_new_deployment` tool with the Git SHA or tag and the repository ID to inform LinearB that a deployment has occurred.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linearb](https://vinkius.com/mcp/linearb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LinearB** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `linearb` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LinearB** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "linearb": {
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
