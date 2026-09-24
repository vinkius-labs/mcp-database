# Family Member Count MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-member-count)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze household composition and member counts.

## Description
This MCP server provides tools to manage and analyze household data. It allows AI agents to determine the total number of residents using `get_household_size`, list specific members and their roles via `get_household_composition`, verify if a household meets registration requirements with `validate_household_completeness`, and filter residents by age groups like minors or seniors using `filter_members_by_age_group`.


## Available Tools (4)
- **get_household_composition**: Who are the members of this household and what are their roles?
- **filter_members_by_age_group**: How many children or adults are in this household?
- **get_household_size**: How many people live in this specific household?
- **validate_household_completeness**: Is the household data sufficient for official registration?


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Member Count** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many people live in household ID 12345?"

**🤖 AI Agent:**
> There are 4 people living in household 12345.

---

**👤 You:**
> "Who are the members of household 98765?"

**🤖 AI Agent:**
> The members of household 98765 are John (Parent), Jane (Parent), and Alex (Child).

---

**👤 You:**
> "Is household 55555 complete for registration if it needs a Parent?"

**🤖 AI Agent:**
> Yes, household 55555 is complete as it contains the required Parent role.


## ❓ FAQ

**Q: How do I check the total number of people in a household?**
You can use the `get_household_size` tool by providing the specific household identifier.

**Q: Can I see the roles of each family member?**
Yes, the `get_household_composition` tool returns a list of all unique members and their assigned roles.

**Q: How can I count only the adults in a household?**
Use the `filter_members_by_age_group` tool and specify 'adult' as the target age group.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-member-count](https://vinkius.com/en/ai-agent-connect/family-member-count)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Member Count** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-member-count` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Member Count** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-member-count": {
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
