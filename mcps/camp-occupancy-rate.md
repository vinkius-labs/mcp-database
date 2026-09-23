# Camp Occupancy Rate MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/camp-occupancy-rate)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Calculate campground occupancy, availability, and usage trends.

## Description
This MCP server provides tools to monitor campground capacity and usage. Use `get_campground_occupancy` to find the current occupancy percentage and total capacity, `get_occupancy_trends` to compare usage across different locations, `validate_site_availability` to check if enough sites are free for a booking, and `get_campground_summary` for a high-level overview of a site's status.


## Available Tools (4)
- **get_campground_summary**: Provides a high-level overview of a campground's current state
- **get_occupancy_trends**: Retrieves occupancy data across multiple campgrounds to compare usage
- **get_campground_occupancy**: Calculates the current occupancy percentage for a specific campground
- **validate_site_availability**: Checks if a specific campground has enough capacity to accommodate a requested number of sites


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Camp Occupancy Rate** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the occupancy rate for campground ID 'forest-01'?"

**🤖 AI Agent:**
> The occupancy rate for forest-01 is 75%, with 75 occupied sites and 25 available sites out of a total capacity of 100.

---

**👤 You:**
> "Is there enough space for 5 sites at campground 'lake-side-42'?"

**🤖 AI Agent:**
> Yes, there are 12 sites available, so you can book 5 sites. You will have 7 sites remaining.

---

**👤 You:**
> "Give me a summary of the status for campground 'mountain-retreat'."

**🤖 AI Agent:**
> The campground 'mountain-retreat' has 50 total sites and a usage ratio of 0.80. It is not full.


## ❓ FAQ

**Q: How is the occupancy rate calculated?**
The occupancy rate is the number of occupied sites divided by the total capacity (occupied plus available sites), expressed as a percentage.

**Q: Can I check if a specific number of sites are available?**
Yes, you can use the `validate_site_availability` tool to check if a campground has enough vacant sites to meet your request.

**Q: How do I see trends across multiple campgrounds?**
You can use `get_occupancy_trends` to retrieve a list of campgrounds and their current occupancy status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/camp-occupancy-rate](https://vinkius.com/en/ai-agent-connect/camp-occupancy-rate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Camp Occupancy Rate** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `camp-occupancy-rate` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Camp Occupancy Rate** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "camp-occupancy-rate": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
