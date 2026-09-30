# Family Photo Sharing Logic Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-photo-sharing-logic-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Manages photo album access using consent, audience groups, and expiration rules.

## Description
This MCP server provides a logic engine for managing photo privacy and sharing permissions. It allows AI agents to determine which recipients can view specific albums by evaluating consent flags, audience group memberships, and temporal constraints. Use `analyze_sharing_permissions` to identify allowed and blocked recipients, `validate_audience_access` to check group membership, `get_share_expiration_calendar` to track access expiry, and `check_temporal_constraints` to verify if an album is within its valid sharing window.


## Available Tools (4)
- **validate_audience_access**: Checks if a specific user is a member of an audience group permitted to view an album
- **analyze_sharing_permissions**: Determines which specific recipients are allowed to view a given album based on all privacy and preference rules
- **check_temporal_constraints**: Verifies if an album's date range allows for sharing based on the current date
- **get_share_expiration_calendar**: Generates a schedule of when existing shares for a specific album will cease to be valid


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Photo Sharing Logic Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Who is allowed to see album 'vacation_2023' among users 'user_1', 'user_2', and 'user_3'?"

**🤖 AI Agent:**
> The allowed recipients for album 'vacation_2023' are 'user_1' and 'user_3'. 'user_2' is blocked due to privacy settings.

---

**👤 You:**
> "Is the album created on '2023-01-01' still valid for sharing today, '2024-05-20'?"

**🤖 AI Agent:**
> Yes, the album is within its valid sharing window.

---

**👤 You:**
> "When will access to album 'family_reunion' expire for recipient 'user_99'?"

**🤖 AI Agent:**
> Access for 'user_99' to the 'family_reunion' album is set to expire on 2024-12-31.


## ❓ FAQ

**Q: How does the system handle blocked users?**
The `analyze_sharing_permissions` tool identifies blocked recipients by checking the user's explicit block list and individual consent flags.

**Q: Can I see when a user's access will expire?**
Yes, you can use `get_share_expiration_calendar` to retrieve a schedule of all upcoming expiration dates for an album.

**Q: How are audience groups verified?**
The `validate_audience_access` tool verifies if a specific user is a member of a permitted audience group.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-photo-sharing-logic-engine](https://vinkius.com/en/ai-agent-connect/family-photo-sharing-logic-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Photo Sharing Logic Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-photo-sharing-logic-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Photo Sharing Logic Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-photo-sharing-logic-engine": {
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
