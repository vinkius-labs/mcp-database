# Digital Legacy Update Log MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/digital-legacy-update-log)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Maintain an auditable, chronological record of digital asset changes, including account status, custodian shifts, and instruction versions.

## Description
This MCP server provides the essential tools to manage a digital legacy audit trail. It allows for tracking changes to account status, managing custodian transitions, and versioning instructional documents. Use `get_account_summary` to check current states, `log_legacy_update` to record new events, `get_audit_history` to review the full timeline, and `verify_review_cycle` to ensure periodic compliance checks are performed.


## Available Tools (4)
- **get_audit_history**: Provides a chronological list of all events associated with an account to facilitate auditing
- **log_legacy_update**: Records a new event (change in account, custodian, or instruction) to the audit log
- **verify_review_cycle**: Checks if an account is due for a mandatory review based on its last recorded review date
- **get_account_summary**: Retrieves the most recent status and core details for a specific digital account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Digital Legacy Update Log** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current status of account ACC-123?"

**🤖 AI Agent:**
> The current status of account ACC-123 is Active, with the latest instruction version being v2.1.

---

**👤 You:**
> "Log a status change for account ACC-456 to Frozen."

**🤖 AI Agent:**
> The status change for account ACC-456 has been successfully recorded in the audit log.

---

**👤 You:**
> "Show me the history for account ACC-789."

**🤖 AI Agent:**
> The history for account ACC-789 shows three events: a status change, a custodian update, and a recent review confirmation.


## ❓ FAQ

**Q: How do I record a change in a custodian?**
You can use the `log_legacy_update` tool with the `CUSTODIAN_CHANGE` update type and provide the `newCustodianId`.

**Q: How can I check if an account needs a review?**
Use the `verify_review_cycle` tool by providing the account ID and the required review frequency in days.

**Q: Can I see the full history of an account?**
Yes, the `get_audit_history` tool provides a complete chronological list of all recorded events for a specific account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/digital-legacy-update-log](https://vinkius.com/en/ai-agent-connect/digital-legacy-update-log)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Digital Legacy Update Log** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `digital-legacy-update-log` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Digital Legacy Update Log** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "digital-legacy-update-log": {
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
