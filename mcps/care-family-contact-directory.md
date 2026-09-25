# Care Family Contact Directory MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/care-family-contact-directory)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Secure contact management for family and healthcare providers with role-based access.

## Description
This MCP server provides a secure management system for organizing contact information for family members and healthcare providers. It enforces privacy through role-based visibility and ensures data accuracy via stale-record auditing. Use `get_directory_view` to access filtered contact lists based on permission tiers, `get_emergency_contacts` for immediate crisis response, `get_stale_records_report` to identify outdated information, and `get_verification_checklist` for quarterly audits.


## Available Tools (4)
- **get_directory_view**: You must provide the requester's role and permission tier.

Provides a filtered view of the contact directory based on the requester's role and permissions
- **get_emergency_contacts**: You can optionally filter by priority level.

Retrieves a highly condensed list of essential contacts specifically for immediate crisis response
- **get_stale_records_report**: Identifies contacts whose information has not been verified within the required maintenance window
- **get_verification_checklist**: Generates a structured list of tasks for a quarterly audit to ensure all contact information is current


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Care Family Contact Directory** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the contact directory for a user with Tier 2 access."

**🤖 AI Agent:**
> Here is the contact directory view for Tier 2 access: [List of names and primary contact methods].

---

**👤 You:**
> "Which contacts have not been verified in the last 90 days?"

**🤖 AI Agent:**
> The following contacts are considered stale: John Doe (last verified 120 days ago), Jane Smith (last verified 105 days ago).

---

**👤 You:**
> "Give me the emergency contact list."

**🤖 AI Agent:**
> The primary emergency contacts are: Alice Johnson (Phone: 555-0123, Priority 1) and Bob Wilson (Phone: 555-0456, Priority 2).


## ❓ FAQ

**Q: How is privacy handled in the directory?**
Privacy is enforced through role-based visibility. Depending on your assigned permission tier, you will only see the contact details permitted for your level of access.

**Q: How can I find contacts that need updating?**
You can use the `get_stale_records_report` tool to identify any contacts whose information has not been verified within your specified timeframe.

**Q: Can I access emergency contacts during a crisis?**
Yes, the `get_emergency_contacts` tool provides a condensed list of essential contacts following the established emergency order, bypassing standard permission tiers for immediate access.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/care-family-contact-directory](https://vinkius.com/en/ai-agent-connect/care-family-contact-directory)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Care Family Contact Directory** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `care-family-contact-directory` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Care Family Contact Directory** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "care-family-contact-directory": {
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
