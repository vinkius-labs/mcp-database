# Rehearsal Space Cost Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/rehearsal-space-cost-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equitably distribute rehearsal facility expenses based on attendance, equipment use, and custom agreements.

## Description
This MCP server provides precise mathematical tools for bands and ensembles to split rehearsal costs fairly. It handles base rental fees, equipment surcharges for specific gear, and credits for deposits already paid. Using `calculate_rehearsal_split`, users can distribute costs based on hours attended or apply custom shares for specific members. It also includes tools like `summarize_total_costs` to view the total liability and `get_participant_participation_ratio` to analyze individual contributions.


## Available Tools (4)
- **calculate_rehearsal_split**: Performs the core mathematical distribution of all rehearsal-related costs among a group of participants
- **get_participant_participation_ratio**: Calculates what percentage of the total effort or time a specific individual contributed
- **summarize_total_costs**: Aggregates all different types of costs into a single overview
- **validate_participant_list**: Ensures that the group of participants and their provided hours/shares are logically consistent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rehearsal Space Cost Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Split a $100 rehearsal fee between Alice (2 hours) and Bob (1 hour). Alice already paid a $20 deposit."

**🤖 AI Agent:**
> Alice owes $46.67 and Bob owes $33.33.

---

**👤 You:**
> "Calculate the total cost for a $50 room rental and a $15 drum kit surcharge."

**🤖 AI Agent:**
> The total combined cost is $65.00.

---

**👤 You:**
> "What is the participation ratio for Charlie if Alice attended 3 hours, Bob 2 hours, and Charlie 5 hours?"

**🤖 AI Agent:**
> Charlie's participation ratio is 0.5.


## ❓ FAQ

**Q: How are the base rental fees distributed?**
The base rental fee is distributed based on the proportion of hours each participant attended, unless a custom share is specified for a member.

**Q: Can I account for equipment usage fees?**
Yes, you can use `calculate_rehearsal_split` to assign specific equipment surcharges to the exact participants who used them.

**Q: How do I handle money already paid to the venue?**
You can input deposits into the `calculate_rehearsal_split` tool. The tool will credit the payer to reduce their final balance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/rehearsal-space-cost-splitter](https://vinkius.com/en/ai-agent-connect/rehearsal-space-cost-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rehearsal Space Cost Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rehearsal-space-cost-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rehearsal Space Cost Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rehearsal-space-cost-splitter": {
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
