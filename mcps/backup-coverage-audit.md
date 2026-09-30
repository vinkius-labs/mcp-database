# Backup Coverage Audit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/backup-coverage-audit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Audit backup configurations to identify protection gaps, staleness, and redundancy.

## Description
This MCP server provides a comprehensive auditing engine for enterprise backup environments. It connects AI agents to your backup infrastructure to identify security gaps and operational risks. Use `analyze_coverage_tool` to find unprotected assets, `check_staleness_tool` to detect failed or outdated backup jobs, `audit_redundancy_tool` to find wasted storage from duplicate data, and `verify_retention_compliance_tool` to ensure data is being purged according to policy.


## Available Tools (4)
- **audit_redundancy_tool**: Detect wasted storage by finding duplicate data sets across different destinations
- **check_staleness_tool**: Find backup jobs that have failed to run or complete within their required frequency
- **verify_retention_compliance_tool**: Ensure that backup retention rules are being honored and that old data is being purged
- **analyze_coverage_tool**: Identify which critical data assets are missing backup protection


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Backup Coverage Audit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which folders are currently unprotected in the production environment?"

**🤖 AI Agent:**
> The following folders in the production environment are unprotected: /data/finance/2023 and /logs/system_critical.

---

**👤 You:**
> "Are there any stale backups older than 7 days?"

**🤖 AI Agent:**
> Yes, the 'Daily_Database_Backup' is stale; its last successful completion was 10 days ago.

---

**👤 You:**
> "Check if the retention policy 'POL-99' is being followed correctly."

**🤖 AI Agent:**
> Policy 'POL-99' is compliant. 150 items were correctly retained and 0 items were erroneously kept or deleted.


## ❓ FAQ

**Q: How can I find unprotected data assets?**
You can use the `analyze_coverage_tool` to identify which critical folders or devices are missing active backup protection.

**Q: How do I detect if my backups are outdated?**
Use the `check_staleness_tool` by providing a maximum age threshold in days to find backup sets that have not completed successfully within the required window.

**Q: Can this tool help reduce storage costs?**
Yes, the `audit_redundancy_tool` identifies duplicate data sets across different destinations, allowing you to consolidate storage and reduce waste.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/backup-coverage-audit](https://vinkius.com/en/ai-agent-connect/backup-coverage-audit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Backup Coverage Audit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `backup-coverage-audit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Backup Coverage Audit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "backup-coverage-audit": {
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
