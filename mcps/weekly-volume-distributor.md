# Weekly Volume Distributor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/weekly-volume-distributor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Distributes weekly training volume across sessions based on muscle group targets and split types.

## Description
This MCP server provides advanced tools for training program design. It allows AI agents to calculate optimal weekly volume distribution using `calculate_volume_distribution`, identify unintended muscle stimulation with `analyze_muscle_overlap`, assess overtraining risks via `get_fatigue_risk_score`, and ensure program logic with `validate_split_feasibility`. It manages muscle group overlap and fatigue to create balanced training schedules.


## Available Tools (4)
- **analyze_muscle_overlap**: Identifies secondary muscle group stimulation resulting from primary muscle group training
- **validate_split_feasibility**: Checks if the requested weekly volume can be realistically distributed within the constraints of the chosen split
- **calculate_volume_distribution**: Generates a complete weekly training schedule by distributing total weekly sets across the specified training days and split type
- **get_fatigue_risk_score**: Evaluates the likelihood of overtraining based on the density of volume and the frequency of sessions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weekly Volume Distributor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Distribute 12 sets for chest and 10 sets for back over 3 days using a push_pull_legs split."

**🤖 AI Agent:**
> Day 1 (Push): Chest 6 sets, Triceps 3 sets. Day 2 (Pull): Back 5 sets, Biceps 5 sets. Day 3 (Legs): No chest or back scheduled.

---

**👤 You:**
> "Is it feasible to do 30 sets of chest in a 2-day full_body split?"

**🤖 AI Agent:**
> No, that volume is not biologically practical for a single session within a 2-day split.

---

**👤 You:**
> "What muscles are worked when I train chest?"

**🤖 AI Agent:**
> Training chest primarily stimulates the pectoralis major, with significant secondary stimulation to the triceps and anterior deltoids.


## ❓ FAQ

**Q: How does the volume distribution work?**
The `calculate_volume_distribution` tool takes your target weekly sets and spreads them across your training days according to your chosen split type, like Push/Pull/Legs or Full Body.

**Q: Can I check if my training plan is too intense?**
Yes, you can use `get_fatigue_risk_score` to evaluate the likelihood of overtraining based on volume density and training frequency.

**Q: Does it account for muscle overlap?**
Yes, the `analyze_muscle_overlap` tool identifies secondary muscle groups that are stimulated during primary movements to prevent accidental overtraining.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/weekly-volume-distributor](https://vinkius.com/en/ai-agent-connect/weekly-volume-distributor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Weekly Volume Distributor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `weekly-volume-distributor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Weekly Volume Distributor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "weekly-volume-distributor": {
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
