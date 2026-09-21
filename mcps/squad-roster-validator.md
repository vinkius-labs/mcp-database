# Squad Roster Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/squad-roster-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [management](../categories/management.md)

Validates football competition rosters for compliance with age, size, and homegrown rules.

## Description
This MCP server provides a specialized validation engine for football (soccer) competition rosters. It ensures compliance with complex regulatory frameworks including age categories, squad size limits, registration deadlines, and nationality or homegrown quotas. Use `validate_roster` to perform full regulatory checks, `check_position_coverage` to verify positional depth, `verify_homegrown_status` to check local talent requirements, and `get_normalized_roster` to generate a clean list of player identities.


## Available Tools (4)
- **check_position_coverage**: Analyzes if the submitted squad has the necessary depth in each positional group
- **get_normalized_roster**: Produces a consistent, stripped-down view of the squad for external reporting
- **validate_roster**: Performs the full suite of regulatory checks to determine if a squad is legal for competition
- **verify_homegrown_status**: Calculates the compliance of a squad regarding local talent requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Squad Roster Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate this roster for competition ID 'league_pro_2024' with player IDs ['p1', 'p2', 'p3'] on 2024-05-01."

**🤖 AI Agent:**
> The roster is valid. No violations or warnings were found for the specified competition.

---

**👤 You:**
> "Check if these players meet the homegrown requirement of 3 players: ['p1', 'p2', 'p3', 'p4']."

**🤖 AI Agent:**
> The squad is compliant. The homegrown count is 3.

---

**👤 You:**
> "Does the squad ['p1', 'p2'] cover the required positions: 'Goalkeeper' and 'Defender'?"

**🤖 AI Agent:**
> Yes, the required positions are covered.


## ❓ FAQ

**Q: What does the validator check?**
The `validate_roster` tool checks squad size, age requirements, registration deadlines, homegrown quotas, and position coverage.

**Q: How can I check if my team has enough goalkeepers?**
You can use the `check_position_coverage` tool by providing the player IDs and the required positions.

**Q: Can I get a clean list of players without registration metadata?**
Yes, use the `get_normalized_roster` tool to receive a consistent list of player identities and primary positions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/squad-roster-validator](https://vinkius.com/en/ai-agent-connect/squad-roster-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Squad Roster Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `squad-roster-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Squad Roster Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "squad-roster-validator": {
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
