# Reporting Compliance Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/reporting-compliance-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [compliance](../categories/compliance.md)

Automated regulatory reporting schedules and compliance tracking for oil and gas operations.

## Description
This MCP server provides a centralized system for managing regulatory obligations in the oil and gas industry. It synthesizes federal, state, and local mandates into a single actionable timeline. Users can use `get_regulatory_calendar` to view upcoming deadlines, `list_report_requirements` to understand specific documentation needs, and `check_compliance_gap` to identify overdue filings or operational risks. It also includes `search_regulatory_database` to query the underlying rules governing specific jurisdictions and operation types.


## Available Tools (4)
- **check_compliance_gap**: Compares current operational data or completed tasks against the required regulatory schedule to identify missing filings or upcoming risks
- **get_regulatory_calendar**: Provides a comprehensive schedule of all reporting deadlines and associated tasks for a specific operational profile
- **list_report_requirements**: Details the specific data points and documentation needed to satisfy a particular regulatory report
- **search_regulatory_database**: Allows users to query the underlying regulatory rules to understand why certain requirements exist


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reporting Compliance Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the reporting deadlines for upstream operations in Texas."

**🤖 AI Agent:**
> Your upcoming deadlines for Texas Upstream operations include the EPA Emissions Report due on March 15th and the State Water Usage Report due on April 10th.

---

**👤 You:**
> "What documents do I need for the Federal Methane Report?"

**🤖 AI Agent:**
> The Federal Methane Report requires continuous monitoring data, equipment calibration logs, and a signed certification of accuracy.

---

**👤 You:**
> "Are there any compliance gaps for my midstream operations in Oklahoma?"

**🤖 AI Agent:**
> Yes, you have one overdue task: the Quarterly Pipeline Integrity Report for the previous quarter is currently missing.


## ❓ FAQ

**Q: How does the tool handle different levels of government?**
The system aggregates requirements from the entire regulatory hierarchy, ensuring that federal, state, and local mandates are all represented in your compliance schedule.

**Q: Can I check for missing reports?**
Yes, you can use the `check_compliance_gap` tool to compare your completed tasks against required deadlines to identify any missing filings.

**Q: What information is needed to get a reporting schedule?**
To use `get_regulatory_calendar`, you must provide the jurisdiction and the operation type, such as Upstream or Midstream.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/reporting-compliance-calendar](https://vinkius.com/en/ai-agent-connect/reporting-compliance-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reporting Compliance Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reporting-compliance-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reporting Compliance Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reporting-compliance-calendar": {
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
