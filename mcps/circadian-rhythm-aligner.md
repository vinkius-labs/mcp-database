# Circadian Rhythm Aligner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/circadian-rhythm-aligner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Gradually shift your feeding window to match new sleep patterns without metabolic shock.

## Description
The Circadian Rhythm Aligner helps you transition your eating schedule smoothly. By using tools like `generate_transition_schedule`, you can calculate a day-by compatible plan that avoids the physiological stress of abrupt changes. You can also use `assess_transition_intensity` to check if your proposed shift is gentle, moderate, or aggressive, and `calculate_shift_magnitude` to find the exact minutes needed for the adjustment.


## Available Tools (3)
- **generate_transition_schedule**: Generate a day-by-day feeding schedule for a transition
- **assess_transition_intensity**: Assess the metabolic risk of a proposed time shift
- **calculate_shift_magnitude**: Calculate the total minutes to shift between two times


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Circadian Rhythm Aligner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I currently start eating at 08:00, but I want to move it to 12:00 over the next 4 days. Can you give me a schedule?"

**🤖 AI Agent:**
> Day 1: 09:00, Day 2: 10:00, Day 3: 11:00, Day 4: 12:00.

---

**👤 You:**
> "Is a 5-hour shift over 2 days considered safe?"

**🤖 AI Agent:**
> A 5-hour shift over 2 days results in a 2.5-hour daily change, which is categorized as Aggressive risk.

---

**👤 You:**
> "How many minutes are between 07:30 and 10:45?"

**🤖 AI Agent:**
> The total shift magnitude is 195 minutes.


## ❓ FAQ

**Q: How does the transition schedule work?**
The `generate_transition_schedule` tool calculates a daily increment based on your current and target start times, spreading the change over several days to prevent metabolic shock.

**Q: What is metabolic shock?**
Metabolic shock is the physiological stress caused by sudden changes in feeding windows, which can disrupt hormones like insulin and cortisol.

**Q: Can I check if my plan is too aggressive?**
Yes, you can use the `assess_transition_intensity` tool to determine if your daily rate of change falls into the Gentle, Moderate, or Aggressive category.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/circadian-rhythm-aligner](https://vinkius.com/mcp/circadian-rhythm-aligner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Circadian Rhythm Aligner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `circadian-rhythm-aligner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Circadian Rhythm Aligner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "circadian-rhythm-aligner": {
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
