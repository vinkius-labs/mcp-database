# Lineup Formation Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/lineup-formation-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [tactical-analysis](../categories/tactical-analysis.md)

Verify football starting lineups against tactical formations and squad rules.

## Description
This MCP server provides a specialized validation engine for football (soccer) tactical analysis. It allows AI agents to audit starting lineups against specific formation templates like 4-4-2 or 4-3-3. Using the `validate_lineup` tool, agents can check for positional requirements, duplicate players, and squad eligibility. Additionally, the `check_squad_composition` tool ensures the total match squad stays within registration limits, while `get_positional_distribution` and `verify_formation_integrity` provide deep insights into tactical alignment and positional counts.


## Available Tools (4)
- **check_squad_composition**: Validates if the total match squad complies with registration limits
- **get_positional_distribution**: Analyzes a group of players to see how they are distributed across tactical roles
- **validate_lineup**: Performs a comprehensive audit of a starting lineup against a provided formation template and squad rules
- **verify_formation_integrity**: Compares a calculated distribution against a required formation to identify specific tactical mismatches


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lineup Formation Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate a 4-4-2 lineup with these players: [GK: Smith, DF: Jones, DF: Brown, DF: Taylor, DF: Wilson, MF: Davis, MF: Miller, MF: Moore, MF: White, FW: Hall, FW: Young]. Squad: [Smith, Jones, Brown, Taylor, Wilson, Davis, Miller, Moore, White, Hall, Young, Green]. Bench: [Black]."

**🤖 AI Agent:**
> The lineup is valid and matches the 4-4-2 formation requirements.

---

**👤 You:**
> "Check if a squad of 25 players is within the limit of 23."

**🤖 AI Agent:**
> The squad exceeds the limit by 2 players.

---

**👤 You:**
> "Analyze the positional distribution for these players: [Role: Center Back, Role: Winger, Role: Striker]."

**🤖 AI Agent:**
> The distribution is: Defender: 1, Midfielder: 1, Forward: 1.


## ❓ FAQ

**Q: How do I validate a specific formation?**
You can use the `validate_lineup` tool by providing the formation template, the starting eleven, the full squad, and the bench players.

**Q: Can I check if my squad size is legal?**
Yes, the `check_squad_composition` tool is designed to verify if the total match squad complies with your specified maximum squad size.

**Q: What happens if a player is in both the starting lineup and the bench?**
The `validate_lineup` tool will detect this as an error and flag the lineup as invalid.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/lineup-formation-validator](https://vinkius.com/en/ai-agent-connect/lineup-formation-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lineup Formation Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lineup-formation-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lineup Formation Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lineup-formation-validator": {
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
