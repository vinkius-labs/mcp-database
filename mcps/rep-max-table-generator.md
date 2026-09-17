# Rep Max Table Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/rep-max-table-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates complete rep max percentage tables, intensity zones, and warm-up sequences.

## Description
This MCP server provides specialized tools for strength training planning. It allows AI agents to calculate precise weight breakdowns for 1-12 repetitions, identify specific intensity zones for strength, hypertrophy, or endurance, and generate progressive warm-up sequences. Use `generate_rep_table` to get a full weight breakdown, `estimate_one_rep_max` to predict maximum capacity from submaximal lifts, `get_zone_recommendations` for goal-specific weight ranges, and `calculate_warmup_sequence` to prepare for heavy sets.


## Available Tools (4)
- **calculate_warmup_sequence**: 
- **estimate_one_rep_max**: 
- **generate_rep_table**: 
- **get_zone_recommendations**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rep Max Table Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I lifted 100kg for 5 reps. What is my estimated 1RM?"

**🤖 AI Agent:**
> Your estimated 1RM is 112.5kg.

---

**👤 You:**
> "Generate a rep table for a 200kg squat."

**🤖 AI Agent:**
> For a 200kg squat, your 1-12 rep weights are: 1 rep: 200kg, 2 reps: 190kg, 3 reps: 180kg, 4 reps: 170kg, 5 reps: 160kg, 6 reps: 150kg, 7 reps: 140kg, 8 reps: 130kg, 9 reps: 120kg, 10 reps: 110kg, 11 reps: 100kg, 12 reps: 90kg.

---

**👤 You:**
> "What weight should I use for hypertrophy if my 1RM is 150kg?"

**🤖 AI Agent:**
> For hypertrophy, you should use a weight between 105kg and 120kg for a rep range of 8-12 reps.


## ❓ FAQ

**Q: How do I estimate my 1RM?**
You can use the `estimate_one_rep_max` tool by providing the weight you lifted and the number of repetitions you completed.

**Q: Can I get specific weights for hypertrophy training?**
Yes, use `get_zone_recommendations` with the target goal set to 'hypertrophy' to find the ideal weight and rep ranges.

**Q: Does this tool provide warm-up sets?**
Yes, the `calculate_warmup_sequence` tool generates a progressive series of sets to prepare you for your target weight.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/rep-max-table-generator](https://vinkius.com/en/ai-agent-connect/rep-max-table-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rep Max Table Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rep-max-table-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rep Max Table Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rep-max-table-generator": {
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
