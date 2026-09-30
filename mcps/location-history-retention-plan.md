# Location History Retention Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/location-history-retention-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Categorize location records into keep, review, or delete-on buckets based on user-defined retention policies.

## Description
This MCP server acts as a classification engine for sensitive geographic telemetry data. It allows AI agents to apply lifecycle policies to location records by filtering through dimensions like date, provider, and device. Using tools like `analyze_retention_plan` and `filter_by_provider_device`, agents can organize data into actionable buckets: Keep, Review, or Delete-On, without performing destructive deletions. This ensures data lifecycle management is handled with precision and user-defined control.


## Available Tools (4)
- **analyze_retention_plan**: Evaluates a set of location records against a user's retention rules to categorize them
- **calculate_retention_expiration**: Determines the exact date a specific record is scheduled to be flagged for deletion
- **filter_by_provider_device**: Narrow down a subset of records to a specific provider or device before applying retention analysis
- **summarize_retention_status**: Provides a high-level count and statistical breakdown of how many records fall into each bucket


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Location History Retention Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these location records using a 30-day retention policy."

**🤖 AI Agent:**
> The analysis is complete. 45 records are marked to Keep, 12 are in Review, and 5 are flagged as Delete-On.

---

**👤 You:**
> "How many records are scheduled for deletion based on my current plan?"

**🤖 AI Agent:**
> There are currently 8 records in the Delete-On bucket.

---

**👤 You:**
> "Calculate the expiration date for a record from January 1st, 2024, with a 90-day retention period."

**🤖 AI Agent:**
> The record is scheduled to be flagged for deletion on March 31st, 2024.


## ❓ FAQ

**Q: Does this tool delete my location data?**
No. This tool is a classification engine. It flags records for future deletion using the `analyze_retention_plan` tool, but it does not perform the actual deletion.

**Q: How can I filter records by a specific device?**
You can use the `filter_by_provider_device` tool to narrow down your records to a specific device ID before running a full retention analysis.

**Q: What are the different retention buckets?**
Records are categorized into Keep (preserved), Review (gray area/approaching expiration), or Delete-On (ready for removal).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/location-history-retention-plan](https://vinkius.com/en/ai-agent-connect/location-history-retention-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Location History Retention Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `location-history-retention-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Location History Retention Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "location-history-retention-plan": {
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
