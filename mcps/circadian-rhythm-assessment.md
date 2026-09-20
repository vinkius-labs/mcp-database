# Circadian Rhythm Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/circadian-rhythm-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Determine your biological chronotype and optimize your sleep schedule.

## Description
This MCP server provides a complete toolkit for understanding your biological clock. By using tools like `get_chronotype_profile` and `calculate_alignment_metrics`, you can identify your specific chronotype, measure the social jetlag caused by your daily schedule, and receive personalized advice through `get_sleep_recommendations`. It also allows for refining your circadian model using `analyze_alertness_patterns` to find your peak productivity windows.


## Available Tools (4)
- **analyze_alertness_patterns**: Pass alertnessData as a JSON string representing an array of {timeOfDay: string, alertnessLevel: number} objects.

Correlates MEQ results with subjective alertness reports to refine the circadian model
- **calculate_alignment_metrics**: Measures how well the user's biological rhythm matches their current lifestyle
- **get_chronotype_profile**: Determines the user's biological chronotype and provides fundamental sleep timing characteristics
- **get_sleep_recommendations**: Provides actionable behavioral advice to minimize misalignment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Circadian Rhythm Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my chronotype if my MEQ score is 75?"

**🤖 AI Agent:**
> Your chronotype is Extreme Morningness, with a peak alertness period in the early morning.

---

**👤 You:**
> "I have an MEQ score of 50, wake up at 07:00, but must wake up at 06:00. How misaligned am I?"

**🤖 AI Agent:**
> Your misalignment score is low, but you are experiencing a slight social jetlag due to the one-hour difference between your preference and requirement.

---

**👤 You:**
> "Give me sleep recommendations for an MEQ score of 30 and a misalignment score of 15."

**🤖 AI Agent:**
> Your primary strategy is Light Exposure Management. You should seek bright light in the late morning to help advance your circadian phase.


## ❓ FAQ

**Q: What is a chronotype?**
A chronotype is your body's natural inclination to sleep or be awake at certain times of the day, such as being a 'Morning Lark' or a 'Night Owl'.

**Q: How do I use the misalignment tool?**
You can use `calculate_alignment_metrics` by providing your MEQ score and your current and required wake times to see how much your schedule conflicts with your biology.

**Q: Can this help me improve my productivity?**
Yes, by using `analyze_alertness_patterns`, you can identify your peak alertness periods to schedule important tasks when you are most awake.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/circadian-rhythm-assessment](https://vinkius.com/en/ai-agent-connect/circadian-rhythm-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Circadian Rhythm Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `circadian-rhythm-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Circadian Rhythm Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "circadian-rhythm-assessment": {
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
