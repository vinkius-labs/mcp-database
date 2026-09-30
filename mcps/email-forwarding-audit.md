# Email Forwarding Audit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/email-forwarding-audit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Audit email forwarding rules to detect unapproved destinations and compliance conflicts.

## Description
This MCP server provides tools to audit mailbox forwarding rules for security and compliance. It allows security teams to identify active rules pointing to unapproved destinations, find inactive rules, and detect compliance conflicts. Use `get_approved_rules` to verify compliant rules, `get_unapproved_destinations` to find potential exfiltration points, `get_inactive_rules` to review disabled configurations, and `identify_compliance_conflicts` to pinpoint high-risk policy violations.


## Available Tools (4)
- **get_unapproved_destinations**: Identifies all destinations used in existing rules that are not on the authorized list
- **get_approved_rules**: Retrieves all forwarding rules that meet the organization's compliance criteria
- **get_inactive_rules**: Identifies all forwarding rules that are currently disabled
- **identify_compliance_conflicts**: Performs a cross-check to find active rules that violate security policies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Email Forwarding Audit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all the forwarding rules that are currently approved."

**🤖 AI Agent:**
> The approved forwarding rules are: Rule ID 101 (destination: internal@company.com), Rule ID 105 (destination: partner@trusted.com).

---

**👤 You:**
> "Are there any active rules pointing to unapproved email addresses?"

**🤖 AI Agent:**
> Yes, there is one unapproved destination being used: attacker@external.com.

---

**👤 You:**
> "Find any high-risk compliance conflicts."

**🤖 AI Agent:**
> A high-risk conflict was found: Rule ID 202 is active and points to an unverified external domain.


## ❓ FAQ

**Q: How do I find rules that violate security policies?**
You can use the `identify_compliance_conflicts` tool to find active rules that point to unverified destinations or have overly broad conditions.

**Q: Can I filter the audit by a specific date range?**
Yes, the `get_approved_rules` tool accepts `minCreationDate` and `maxCreationDate` parameters to define your audit window.

**Q: How are unapproved destinations identified?**
The `get_unapproved_destinations` tool identifies any destination address used in existing rules that is not present in the organization's authorized destination catalog.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/email-forwarding-audit](https://vinkius.com/en/ai-agent-connect/email-forwarding-audit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Email Forwarding Audit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `email-forwarding-audit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Email Forwarding Audit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "email-forwarding-audit": {
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
