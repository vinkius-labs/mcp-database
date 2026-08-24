# Powerlifting Coefficient Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/powerlifting-coefficient-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Calculate and compare strength scores using Wilks, DOTS, and IPF GL coefficients.

## Description
This MCP server provides deterministic tools to normalize powerlifting performance across different weight classes. By using mathematical coefficients, lifters can be compared fairly regardless of their body mass. The server includes tools to `calculate_strength_scores` for Wilks, DOTS, and IPF GL metrics, identify official competition weight classes via `get_weight_class`, and perform comparative analysis using `rank_lifters_by_coefficient`.


## Available Tools (3)
- **calculate_strength_scores**: Calculates standard powerlifting coefficients (Wilks, DOTS, IPF GL) for a lifter
- **rank_lifters_by_coefficient**: Ranks a list of lifters based on a specific coefficient
- **get_weight_class**: Identifies the official competition weight class for a lifter


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Powerlifting Coefficient Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the strength scores for a male lifter weighing 90kg with a 250kg total."

**🤖 AI Agent:**
> The calculated scores for this lifter are: Wilks: 325.4, DOTS: 342.1, and IPF GL: 338.5.

---

**👤 You:**
> "What weight class is a 65kg female lifter in?"

**🤖 AI Agent:**
> A 65kg female lifter belongs to the 63kg Class (range: 60kg - 63kg) or the 69kg Class depending on the specific federation table used.

---

**👤 You:**
> "Rank these lifters by DOTS: [{bodyweight: 70, totalLifted: 400, gender: 'male'}, {bodyweight: 100, totalLifted: 500, gender: 'male'}]"

**🤖 AI Agent:**
> 1. Lifter 1 (Score: 415.2), 2. Lifter 2 (Score: 398.5).


## ❓ FAQ

**Q: What is a DOTS score?**
DOTS is a modern coefficient used to compare strength across different weight classes in powerlifting, providing a more accurate relative strength metric than older systems.

**Q: Can I compare lifters of different genders?**
The tool applies gender-specific polynomial constants to ensure that both male and female lifters receive accurate, physiologically appropriate scores.

**Q: How do I rank multiple athletes at once?**
You can use the `rank_lifters_by_coefficient` tool by providing a list of lifter profiles to receive a sorted ranking based on your chosen coefficient.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/powerlifting-coefficient-calculator](https://vinkius.com/ai-agent-connect/powerlifting-coefficient-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Powerlifting Coefficient Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `powerlifting-coefficient-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Powerlifting Coefficient Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "powerlifting-coefficient-calculator": {
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
