# Golf Handicap Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/golf-handicap-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Deterministic golf handicap calculation per USGA/WHS standards.

## Description
This MCP server provides precise golf handicap calculations following the World Handicap System (WHS). It allows AI agents to determine a player's current Handicap Index using `calculate_handicap_index`, calculate the specific strokes received at a target course via `calculate_course_handicap`, and determine the final playing handicap with environmental adjustments using `calculate_playing_handicap`. The system strictly adheres to Net Double Bogey rules and handles 9-hole score combinations.


## Available Tools (3)
- **calculate_course_handicap**: Determine how many strokes a player will receive at a specific target course
- **calculate_handicap_index**: Determine the player's current Handicap Index based on recent scoring history
- **calculate_playing_handicap**: Determine the final number of strokes a player uses in a round after environmental adjustments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Golf Handicap Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my handicap index for these 20 rounds: [{"grossScore": 85, "courseRating": 72.0, "slopeRating": 113, "par": 72}, ...]"

**🤖 AI Agent:**
> Your current Handicap Index is 14.2.

---

**👤 You:**
> "How many strokes will I get at a course with a 71.5 rating and 130 slope if my handicap index is 15.0?"

**🤖 AI Agent:**
> You will receive 18 strokes at this course.

---

**👤 You:**
> "What is my playing handicap for a course with rating 70.0, slope 120, par 72, given a handicap index of 10.0 and a PCC of 0.0?"

**🤖 AI Agent:**
> Your playing handicap is 12.


## ❓ FAQ

**Q: How is the Handicap Index calculated?**
The index is calculated by taking the average of the best 8 score differentials from the most recent 20 rounds, then multiplying by 0.96.

**Q: What is the maximum score allowed per hole?**
The system applies the Net Double Bogey rule, ensuring no single hole disproportionately affects the handicap.

**Q: Can I calculate my playing handicap for a specific course?**
Yes, you can use `calculate_playing_handicap` to get the final number of strokes after accounting for course rating, slope, and PCC adjustments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/golf-handicap-calculator](https://vinkius.com/ai-agent-connect/golf-handicap-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Golf Handicap Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `golf-handicap-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Golf Handicap Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "golf-handicap-calculator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
