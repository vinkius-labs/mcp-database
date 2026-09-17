# Working Set Weight Selector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/working-set-weight-selector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Dynamically adjust training loads using RPE, fatigue, and performance data.

## Description
Optimize your strength training with real-time auto-regulation. This MCP server connects your training data to intelligent weight selection algorithms. Use `calculate_working_weight` to determine your primary load based on recent performance and fatigue, `generate_warmup_progression` to prepare your body with structured ramp-up sets, `get_intensity_guidance` to identify your training zone, and `validate_session_readiness` to ensure you are training safely. It bridges the gap between subjective feeling and objective training stimulus.


## Available Tools (4)
- **get_intensity_guidance**: Provide qualitative feedback on the perceived difficulty of the planned session
- **calculate_working_weight**: Determine the primary load for the intended training sets
- **generate_warmup_progression**: Provide a ramp-up sequence to prepare for the working weight
- **validate_session_readiness**: Evaluate if the user should proceed with the planned load


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Working Set Weight Selector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I lifted 100kg for 5 reps last time. I want to hit an RPE 8 today, but I feel a bit tired (fatigue level 3). What should my weight be?"

**🤖 AI Agent:**
> Based on your recent performance and current fatigue, your recommended working weight is 92kg.

---

**👤 You:**
> "Give me a warmup for a 120kg squat session."

**🤖 AI Agent:**
> Your warmup progression is: 20kg x 10, 60kg x 5, 90kg x 3, 105kg x 2.

---

**👤 You:**
> "Is it safe to train at RPE 9 if my fatigue level is 8?"

**🤖 AI Agent:**
> No, your fatigue level is too high for that intensity. Rest day recommended.


## ❓ FAQ

**Q: How does the weight selection work?**
The tool uses your recent performance weight, your target RPE, and your current fatigue level to calculate a recommended working weight through an auto-regulation algorithm.

**Q: Can I use this for hypertrophy training?**
Yes, you can use `get_intensity_guidance` to confirm if your chosen RPE and rep goal fall within the hypertrophy training zone.

**Q: What if I feel too tired to train?**
You should use `validate_session_readiness` to check if your current fatigue level makes the intended intensity unsafe.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/working-set-weight-selector](https://vinkius.com/en/ai-agent-connect/working-set-weight-selector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Working Set Weight Selector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `working-set-weight-selector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Working Set Weight Selector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "working-set-weight-selector": {
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
