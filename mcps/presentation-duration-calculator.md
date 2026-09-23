# Presentation Duration Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/presentation-duration-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Estimate presentation length and get pacing recommendations.

## Description
This MCP server provides tools to plan presentation timing accurately. Use `get_estimated_duration` to calculate total time based on slide count and pacing, or `get_pacing_recommendation` to find the ideal time per slide for specific styles like a Quick Pitch or Technical Deep Dive. It also offers `get_presentation_summary` for a high-level overview of your planned session.


## Available Tools (4)
- **get_estimated_duration**: Calculate the total estimated duration of a presentation
- **get_pacing_recommendation**: Get a recommended pacing for a specific presentation tier
- **get_presentation_summary**: Get a summary of the presentation characteristics
- **list_presentation_tiers**: List all available presentation tiers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Presentation Duration Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How long will a 20-slide presentation take if I spend 3 minutes per slide?"

**🤖 AI Agent:**
> The total duration for a 20-slide presentation with 3 minutes per slide is 60 minutes.

---

**👤 You:**
> "What is the recommended pacing for a Technical Deep Dive?"

**🤖 AI Agent:**
> For a Technical Deep Dive, the recommended pacing is 10 minutes per slide.

---

**👤 You:**
> "Give me a summary for 10 slides at 5 minutes each."

**🤖 AI Agent:**
> The presentation will last 50 minutes, which is considered a Long Form presentation.


## ❓ FAQ

**Q: How do I know how much time to spend on each slide?**
You can use the `get_pacing_recommendation` tool to receive a suggested time per slide based on your presentation tier, such as an Educational Session or a Standard Briefing.

**Q: Can I include extra time for Q&A?**
Yes, when using `get_estimated_duration`, you can provide a `bufferMinutes` value to account for questions, technical delays, or transitions.

**Q: What is a 'Long Form' presentation?**
A presentation is categorized as Long Form by the `get_presentation_summary` tool if the total calculated duration is 45 minutes or more.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/presentation-duration-calculator](https://vinkius.com/en/ai-agent-connect/presentation-duration-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Presentation Duration Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `presentation-duration-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Presentation Duration Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "presentation-duration-calculator": {
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
