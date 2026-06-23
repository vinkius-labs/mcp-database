# ParseHub MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/parsehub)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Control advanced cloud scraping projects via ParseHub — list targets, dispatch headless runs, trace crawler status, and fetch extracted datasets directly via AI.

## Description
Bring **ParseHub Cloud Scraping** directly into your AI workflows. Manage pre-configured web scraping targets natively and orchestrate complex headless browser automation directly from chat. Dispatch run jobs on command, query execution status limits, and extract final parsed payloads securely.

### What you can do

- **Project Navigation** — Inspect and list configured ParseHub projects, determining start URLs, templates, and total crawler pages attached
- **Execution Dispatch** — Command remote servers to trigger specific headless data extraction jobs `run_project` optionally overriding starting URLs natively
- **Observability Tracing** — Monitor exactly where a `Run` object is (queued, initialized, running, complete) without checking the desktop app
- **Payload Extraction** — Pull down structured arrays containing the scraped payloads securely via `get_run_data` matching explicit datasets

### How it works

1. Subscribe to this server
2. Enter your ParseHub API Key
3. Start orchestrating complex scraping runs natively from Claude, Cursor, or your MCP UI

### Who is this for?

- **Data Engineers** — trigger cloud scraping logic securely and pipeline extracted datasets straight into processing tools natively
- **Marketing Intel** — fetch completed scrapers watching competitor pricing logic tracking JSON arrays automatically
- **Research Analysts** — kick off academic paper extractors via chat and digest the results upon completion


## Available Tools (10)
- **cancel_run**: If the run was already scraping pages, partial data may be available. Data from already-scraped pages is preserved and can be retrieved with get_run_data. Use this to stop long-running scrapes or free up queue slots.

Cancel a queued or actively running ParseHub run
- **delete_run**: Cannot be undone. Use this to clean up old runs and free up storage quota on your account.

Permanently delete a ParseHub run and its extracted data
- **get_project**: The project_token can be found via list_projects or in the ParseHub desktop client settings tab.

Get detailed configuration of a specific ParseHub project
- **get_run_data**: Only works when the run status is "complete" and data_ready is true. The JSON structure mirrors the template selection configuration set up in the ParseHub desktop client.

Download the raw JSON data extracted from a completed ParseHub run
- **get_run_details**: Poll this endpoint to wait for a run to complete before fetching data.

Check the status of a specific ParseHub run
- **get_last_ready_data**: Ideal for dashboards or integrations that always want the freshest available data without managing individual run tokens.

Instantly get the latest completed data for a ParseHub project
- **list_projects**: Each project includes a project_token (unique identifier), title, last_run timestamp, and template configuration. Use the project_token for all subsequent run management operations.

List all ParseHub web scraping projects
- **list_runs**: Useful for auditing or finding a specific completed run to fetch data from.

Get the history of all runs for a ParseHub project
- **run_project**: Returns a run_token for tracking progress. The run enters a queue and begins processing within seconds. Use get_run to monitor and get_run_data to retrieve results once complete.

Start a new ParseHub scraping run for a project
- **run_project_with_url**: Perfect for scraping different pages with the same template (e.g., different product categories). The template extraction rules still apply unchanged — only the starting page changes.

Start a ParseHub run targeting a custom URL instead of the project default


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ParseHub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the list of scrape projects I have on my ParseHub account."

**🤖 AI Agent:**
> Found 3 mapping projects in your account. 1: 'Pricing Monitor' (Token: t9zx... , runs: 4). 2: 'Real Estate Leads' (Token: t4ax...). 3: 'Competitor Blogs'. Want me to launch any of these into a run?

---

**👤 You:**
> "Start a new run for project 't9zx...' and check its status."

**🤖 AI Agent:**
> Dispatched action `run_project` for target `t9zx...`. Wait, pulling status logic: The cloud system confirmed it. Run ID `run_k1l`. Current Status is 'queued'. The parser will begin explicitly extracting domains soon.

---

**👤 You:**
> "Extract the finished data JSON payload from run ID 'run_k1l'."

**🤖 AI Agent:**
> Pulled exact constraints running `get_run_data`. The JSON indicates 40 records containing titles and strict price fields. Would you like me to process this data or format it differently?


## ❓ FAQ

**Q: Do I need the ParseHub Desktop tool running to use this?**
No. This integration operates completely natively via ParseHub's Cloud API endpoints. You only need the desktop app to build the templates originally. All executions mapped here happen on their cloud scaling servers.

**Q: Can I provide a different Start URL when running a project?**
Yes. The `run_project_with_url` command allows you to explicitly provide a `start_url` query property. This instructs the ParseHub crawler to ignore its project-saved URL and begin parsing the newly mapped domain using the same semantic template.

**Q: Is the downloaded data returned in JSON or raw HTML?**
The payload fetched by `get_run_data` is exported entirely as structured, pre-parsed JSON mirroring the exact template node selections defined in your project architecture.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/parsehub](https://vinkius.com/mcp/parsehub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ParseHub** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `parsehub` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ParseHub** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "parsehub": {
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
