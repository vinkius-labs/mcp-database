# Contact List Merge Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/contact-list-merge-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Identify duplicate contacts and resolve data conflicts within contact datasets.

## Description
This MCP server provides tools to clean and unify contact datasets. Use `analyze_contact_duplicates` to group identical contacts by email, phone, or normalized name. Once groups are identified, use `detect_field_conflicts` to find data discrepancies and `select_primary_record` to deterministically pick the most complete master record for each identity.


## Available Tools (4)
- **analyze_contact_duplicates**: Identifies groups of duplicate contacts based on user-selected matching rules
- **detect_field_conflicts**: Identifies specific data discrepancies within identified merge groups
- **get_normalized_name_summary**: Provides a count of how many unique identities exist when matching specifically by normalized name
- **select_primary_record**: Deterministically picks one record from a group to serve as the master record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Contact List Merge Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all duplicate contacts in this list based on their email addresses."

**🤖 AI Agent:**
> I have identified 3 duplicate groups based on email addresses. There are 5 total duplicate records.

---

**👤 You:**
> "Which contact should be the primary record for the group with ID 'group_123'?"

**🤖 AI Agent:**
> The primary record for group 'group_123' is contact ID 'user_882' because it contains the most complete information.

---

**👤 You:**
> "How many unique identities are there if I match by normalized name?"

**🤖 AI Agent:**
> There are 45 unique identities found among the 50 provided contact records.


## ❓ FAQ

**Q: How does the tool decide which contact is the primary record?**
The `select_primary_record` tool picks the record with the highest completeness (most non-empty fields). If there is a tie, it selects the record with the alphabetically first ID.

**Q: What fields can I use to match contacts?**
You can match contacts using email, phone, or a normalized version of their name via the `analyze_contact_duplicates` tool.

**Q: Can I check for specific field inconsistencies?**
Yes, use `detect_field_conflicts` and provide a list of field names you want to inspect for discrepancies within your merge groups.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/contact-list-merge-plan](https://vinkius.com/en/ai-agent-connect/contact-list-merge-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Contact List Merge Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `contact-list-merge-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Contact List Merge Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "contact-list-merge-plan": {
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
