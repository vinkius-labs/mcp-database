# Account Closure Evidence Register MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/account-closure-evidence-register)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track and audit account closure requests with verifiable evidence.

## Description
This MCP server provides a centralized system for managing the lifecycle of account closure audits. It allows users to register closure requests, track their progress, and record formal evidence once a service confirms a closure. Use `get_register_summary` to view high-level status counts, `register_closure_request` to initiate new entries, `record_closure_evidence` to mark requests as verified, and `get_followup_list` to identify overdue requests requiring attention.


## Available Tools (4)
- **record_closure_evidence**: Updates a pending request with the formal proof of closure
- **get_register_summary**: Provides a high-level overview of the current status of all account closure requests
- **register_closure_request**: Ensure the follow-up date is after the request date.

Adds a new account closure attempt to the register
- **get_followup_list**: Identifies all accounts that require immediate attention because their follow-up date has arrived


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Account Closure Evidence Register** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a summary of all pending account closure requests."

**🤖 AI Agent:**
> There are currently 5 pending account closure requests in the register.

---

**👤 You:**
> "Which account closures need my attention today?"

**🤖 AI Agent:**
> The following requests are overdue: AWS (Full Deletion) and Slack (Subscription Stop).

---

**👤 You:**
> "I have received confirmation for the AWS closure. The reference is REF-12345."

**🤖 AI Agent:**
> The request for AWS has been successfully updated to VERIFIED with confirmation reference REF-12345.


## ❓ FAQ

**Q: How do I see how many requests are still pending?**
You can use the `get_register_summary` tool and filter by the PENDING status to see the current count of requests awaiting verification.

**Q: What should I do if a follow-up date has passed?**
Use the `get_followup_list` tool to identify all requests that are overdue and require immediate verification or action.

**Q: How do I mark a closure as successful?**
Once you receive a confirmation reference from the service, use `record_closure_evidence` to update the request status to VERIFIED.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/account-closure-evidence-register](https://vinkius.com/en/ai-agent-connect/account-closure-evidence-register)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Account Closure Evidence Register** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `account-closure-evidence-register` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Account Closure Evidence Register** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "account-closure-evidence-register": {
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
