# Myo-Reps Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/myo-reps-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate Myo-Reps training parameters including activation sets, mini-sets, and rest pauses.

## Description
This MCP server implements the Myo-Reps protocol based on Borge Fagerli's methodology to maximize hypertrophy. It allows AI agents to calculate precise training structures by determining the initial `get_activation_set_details`, planning the required `calculate_mini_sets_plan`, determining `calculate_rest_pauses`, and summarizing the `get_total_effective_volume`.


## Available Tools (4)
- **calculate_mini_sets_plan**: Calculates how many mini-sets are required to hit the desired hypertrophy goal
- **calculate_rest_pauses**: Determines the total downtime required during the protocol
- **get_activation_set_details**: Determines the starting point and structure of the training session
- **get_total_effective_volume**: Provides the final summary of the completed work


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Myo-Reps Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I just did 12 reps of Bench Press for my activation set. I want to hit 25 effective reps total. How many mini-sets of 4 reps should I do and how much rest?"

**🤖 AI Agent:**
> To reach 25 effective reps after your 12-rep activation set, you need 13 more reps. With 4 reps per mini-set, you will perform 4 mini-sets. This will require 3 rest intervals.

---

**👤 You:**
> "Calculate my Myo-Reps plan for Squats: 10 activation reps, target 20 effective reps, 3 reps per mini-set."

**🤖 AI Agent:**
> For Squats, you will perform 4 mini-sets of 3 reps each to reach your target of 20 effective reps. You will need 3 rest intervals between these mini-sets.

---

**👤 You:**
> "What is the total volume if I do 15 activation reps, 3 mini-sets of 5 reps?"

**🤖 AI Agent:**
> The total volume for your session is 30 repetitions.


## ❓ FAQ

**Q: What is the Myo-Reps protocol?**
Myo-Reps is a high-intensity training method that uses an activation set followed by several mini-sets with short rest pauses to maximize effective repetitions.

**Q: How do I use the calculator?**
Provide the exercise name, the number of reps in your activation set, and your target effective reps to get a complete training plan.

**Q: Can I use this with Claude or Cursor?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/myo-reps-calculator](https://vinkius.com/en/ai-agent-connect/myo-reps-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Myo-Reps Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `myo-reps-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Myo-Reps Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "myo-reps-calculator": {
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
