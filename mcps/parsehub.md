# ParseHub MCP Server

Control advanced cloud scraping projects via ParseHub — list targets, dispatch headless runs, trace crawler status, and fetch extracted datasets directly via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/parsehub)

## Overview
**Category:** developer-tools
**Tools Count:** 10

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


## Available Tools
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


## Installation & Usage

To install and use the **ParseHub** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/parsehub](https://vinkius.com/mcp/parsehub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
