# PhantomBuster MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/phantombuster)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate web data extraction via PhantomBuster — list Phantoms, launch automations, and track results directly from any AI agent.

## Description
Connect your **PhantomBuster** account to any AI agent and take full control of your lead generation and web automation workflows through natural conversation.

### What you can do

- **Agent Oversight** — List all your Phantoms and workflows to maintain visibility over your automation suite.
- **Automation Control** — Launch and abort Phantoms directly through the agent, including support for custom arguments.
- **Result Retrieval** — Fetch the latest outputs and data extracted by your Phantoms for immediate analysis.
- **Configuration Auditing** — Review the setup and arguments of any Phantom to verify your automation logic.
- **Usage Monitoring** — Get account settings and usage info to track your available execution time.

### How it works

1. Subscribe to this server
2. Enter your PhantomBuster API Key
3. Start automating your lead generation from Claude, Cursor, or any MCP client

### Who is this for?

- **Growth Marketers** — quickly launch lead extraction Phantoms or check the results of a LinkedIn automation.
- **Sales Ops** — monitor active workflows and retrieve extracted data for CRM enrichment.
- **Data Engineers** — audit Phantom configurations and results during integration development.


## Available Tools
- **abort_phantom**: Stop a running Phantom
- **get_phantombuster_account**: Get account settings and usage info
- **get_phantom_setup**: Get configuration arguments for a Phantom
- **get_phantom_output**: Get output/results from a Phantom
- **get_phantom**: Get details for a specific Phantom
- **get_workflow**: Get details for a specific workflow
- **launch_phantom**: Start a Phantom execution
- **list_containers**: List all Phantom containers
- **list_phantoms**: List all Phantom agents
- **list_workflows**: List all automation workflows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PhantomBuster** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Phantoms in my account and show their current status."

**🤖 AI Agent:**
> I've retrieved 5 Phantoms: 'LinkedIn Search Export' (Success), 'Sales Navigator Search' (Error), 'Web Scraper' (Ready), and 2 others. Which one would you like to manage?

---

**👤 You:**
> "Launch the 'LinkedIn Search Export' Phantom with ID '12345'."

**🤖 AI Agent:**
> Phantom 'LinkedIn Search Export' (ID: 12345) has been launched successfully. I'll notify you once the output is ready.

---

**👤 You:**
> "Show me the extracted data from the last run of Phantom 12345."

**🤖 AI Agent:**
> I've fetched the results for Phantom 12345. It extracted 150 leads, including names, company titles, and LinkedIn profile URLs. Would you like a detailed breakdown?


## ❓ FAQ

**Q: How do I find my PhantomBuster API Key?**
In your PhantomBuster account, click on your name in the top right, go to **Org settings** or **Workspace settings**, and look for the **API Key** section.

**Q: Can I provide arguments when launching a Phantom?**
Yes! The `launch_phantom` action accepts an optional `argument` field where you can provide a JSON string of parameters to override the default Phantom configuration.

**Q: How do I see the data extracted by a Phantom?**
Use the `get_phantom_output` tool with the specific agent ID. It will return the results of the last successful execution of that Phantom.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/phantombuster](https://vinkius.com/mcp/phantombuster)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PhantomBuster** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `phantombuster` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PhantomBuster** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "phantombuster": {
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
