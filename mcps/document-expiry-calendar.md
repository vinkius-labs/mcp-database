# Document Expiry Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/document-expiry-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Proactive compliance management for document lifecycles and renewal schedules.

## Description
This MCP server provides a proactive compliance management system to track document lifecycles. It calculates renewal windows based on expiry dates and lead times, allowing AI agents to manage renewal schedules effectively. Users can retrieve a chronological `get_renewal_calendar` to see upcoming windows, identify specific tasks for owners via `get_action_owner_tasks`, and lookup specific submission protocols using `get_document_requirements`. For compliance failures, `get_missed_deadline_contingencies` provides risk assessments and remediation steps for expired documents.


## Available Tools (4)
- **get_action_owner_tasks**: Retrieves a list of specific tasks assigned to a particular responsible person
- **get_document_requirements**: Details the specific submission protocols and necessary materials for a document's renewal
- **get_missed_deadline_contingencies**: Identifies documents that have expired and provides the necessary risk assessment and remediation steps
- **get_renewal_calendar**: Provides a chronological schedule of all upcoming renewal windows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Document Expiry Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the renewal schedule for the next three months."

**🤖 AI Agent:**
> Here is your renewal calendar for the next three months: 1. Passport (Starts: 2024-10-15, Expires: 2024-11-15), 2. Driver License (Starts: 2024-12-01, Expires: 2025-01-01).

---

**👤 You:**
> "What are the requirements to renew my Business Permit?"

**🤖 AI Agent:**
> To renew your Business Permit, you must use the digital portal and provide a valid tax certificate and proof of address.

---

**👤 You:**
> "What tasks are assigned to Alice?"

**🤖 AI Agent:**
> Alice has the following upcoming tasks: Renew Health Certificate by 2024-11-20 via digital portal.


## ❓ FAQ

**Q: How are renewal dates calculated?**
The renewal start date is calculated by subtracting the document's specific lead time from its expiry date.

**Q: Can I see tasks assigned to a specific person?**
Yes, you can use the `get_action_owner_tasks` tool to retrieve a list of tasks for a specific responsible owner.

**Q: What happens if a document expires?**
You can use `get_missed_deadline_contingencies` to identify overdue documents and receive risk levels and remediation steps.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/document-expiry-calendar](https://vinkius.com/en/ai-agent-connect/document-expiry-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Document Expiry Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `document-expiry-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Document Expiry Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "document-expiry-calendar": {
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
