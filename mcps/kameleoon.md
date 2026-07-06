# Kameleoon MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kameleoon)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage A/B testing, personalization, and experimentation workflows via AI agents.

## Description
Empower your AI agents to control your **Kameleoon** experimentation platform. This MCP server enables seamless management of experiments, variations, and audience segments directly from natural language interfaces.

### What you can do

- **Experiment Control** — List all active experiments and drill down into specific configurations and metadata
- **Variation Management** — Inspect A/B variations and their statuses across different digital properties
- **Site Inventory** — Query all sites and properties registered in your account to ensure correct environment targeting
- **Audience Segmentation** — List defined audience segments and targeting rules used for precise traffic allocation
- **Results Triggering** — Request latest results reports to analyze experiment performance on the fly

### How it works

1. Subscribe to this server
2. Enter your Kameleoon Client ID and Client Secret
3. Start managing your A/B tests and personalization from Claude, Cursor, or any MCP client

### Who is this for?

- **Product Managers** — Monitor the status of live experiments and check variants without logging into the Kameleoon dashboard
- **Growth Engineers** — Quickly query targeting rules and custom data dimensions from your IDE
- **Data Analysts** — Automate the retrieval of experiment results and metadata for reporting


## Available Tools (10)
- **create_experiment**: Requires a name and a site ID.

Create a new experiment
- **list_custom_data**: List custom data dimensions
- **list_experiments**: Use this to monitor campaign statuses and identify active experiments.

List all experiments in Kameleoon
- **list_sites**: List all sites in the account
- **list_variations**: ) associated with a specific experiment ID.

List variations for an experiment
- **get_experiment**: Get details for a specific experiment
- **get_site**: Get details for a specific site
- **get_experiment_results**: This is an asynchronous process in the Kameleoon API.

Request a results report for an experiment
- **list_targeting_rules**: List targeting rules
- **list_segments**: List audience segments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kameleoon** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all active experiments in my Kameleoon account."

**🤖 AI Agent:**
> I've fetched your experiments. Currently, you have 4 active experiments, including 'New Checkout Flow (AB)' and 'Home Page Personalization'. Which one would you like to inspect?

---

**👤 You:**
> "What are the variations for experiment ID '12345'?"

**🤖 AI Agent:**
> For experiment 12345, I found 3 variations: 'Reference' (Original), 'Variant A (Red Button)', and 'Variant B (Blue Button)'. All variants are currently receiving traffic.

---

**👤 You:**
> "List all sites registered in my Kameleoon profile."

**🤖 AI Agent:**
> I've retrieved 2 sites from your profile: 'Main E-commerce (Code: SEC-123)' and 'Marketing Blog (Code: BLOG-456)'.


## ❓ FAQ

**Q: How can I check if an experiment is currently active on a specific site?**
Use the `list_experiments` tool to get a summary of all experiments, which includes their current status (e.g., 'ACTIVE', 'PAUSED') and assigned site IDs.

**Q: Can I see the defined variations for a particular experiment?**
Yes, the `list_variations` tool takes an experiment ID and returns all variants configured for that test, along with their metadata.

**Q: Is it possible to list targeting rules and segments?**
Absolutely. You can use the `list_segments` and `list_targeting_rules` tools to inspect how your traffic is being allocated across your experimentation ecosystem.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kameleoon](https://vinkius.com/mcp/kameleoon)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kameleoon** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kameleoon` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kameleoon** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kameleoon": {
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
