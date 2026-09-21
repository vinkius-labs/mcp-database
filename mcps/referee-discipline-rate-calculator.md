# Referee Discipline Rate Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/referee-discipline-rate-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Analyze football referee disciplinary patterns, card rates, and impartiality metrics.

## Description
This MCP server provides deep analytical insights into football refereeing behavior. It allows AI agents to calculate disciplinary rates per match, determine how frequently fouls result in cards using `get_referee_foul_punishment_rate`, and assess home/away bias via `get_referee_impartiality_metrics`. Users can also retrieve high-level summaries with `get_referee_discipline_summary` or audit raw data using `get_referee_exact_counts`.


## Available Tools (4)
- **get_referee_exact_counts**: Provides raw, non-normalized totals for all disciplinary categories for auditing
- **get_referee_impartiality_metrics**: Determines if a referee shows a tendency to favor or penalize home or away teams
- **get_referee_discipline_summary**: Provides a high-level overview of a referee's disciplinary impact per match
- **get_referee_foul_punishment_rate**: Measures how frequently a referee penalizes fouls with cards


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Referee Discipline Rate Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the disciplinary summary for referee ID 'ref_123'?"

**🤖 AI Agent:**
> Referee ref_123 has officiated 45 matches and issued a total of 32 cards, resulting in a discipline rate of 0.71 cards per match.

---

**👤 You:**
> "How often does referee 'ref_456' penalize fouls with cards?"

**🤖 AI Agent:**
> Referee ref_456 has a punishment rate of 12.5 cards per 100 fouls.

---

**👤 You:**
> "Does referee 'ref_789' show any home/away bias?"

**🤖 AI Agent:**
> Referee ref_789 shows a home/away card difference of 0.05, indicating very little bias between home and away teams.


## ❓ FAQ

**Q: How can I check if a referee is biased towards home teams?**
You can use the `get_referee_impartiality_metrics` tool to see the difference in card rates between home and away teams.

**Q: What does the cards per 100 fouls metric represent?**
It measures the frequency of card issuance relative to the number of fouls, which helps identify how strict a referee is regardless of match physicality.

**Q: Can I get the exact number of yellow cards issued by a referee?**
Yes, the `get_referee_exact_counts` tool provides raw, unrounded totals for yellow cards, red cards, and other disciplinary events.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/referee-discipline-rate-calculator](https://vinkius.com/en/ai-agent-connect/referee-discipline-rate-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Referee Discipline Rate Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `referee-discipline-rate-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Referee Discipline Rate Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "referee-discipline-rate-calculator": {
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
