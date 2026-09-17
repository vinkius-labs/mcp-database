# RPE to Weight Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/rpe-to-weight-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fitness](../categories/fitness.md)

Convert RPE to training weight and vice versa using standardized intensity tables.

## Description
This MCP server provides strength athletes with precise tools to translate perceived exertion into actionable training loads. By using standardized intensity tables, lifters can use `calculate_target_weight` to find the exact weight needed for a specific RPE and rep count, or `estimate_rpe` to predict how heavy a weight will feel. It also includes `adjust_for_fatigue` to account for strength loss and `get_rep_reserve_info` to quickly translate between RPE and Reps in Reserve (RIR).


## Available Tools (4)
- **adjust_for_fatigue**: Recalculates training targets to account for a reduction in strength caused by fatigue
- **calculate_target_weight**: Determines the specific weight a lifter should use to hit a desired RPE for a given number of repetitions
- **estimate_rpe**: Predicts what the RPE will be when lifting a specific weight for a set number of repetitions
- **get_rep_reserve_info**: Quickly translates between RPE and RIR to help lifters understand their buffer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RPE to Weight Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a 1RM of 300 lbs. What weight should I use for 5 reps at RPE 8?"

**🤖 AI Agent:**
> For a 300 lbs 1RM, 5 reps at RPE 8 requires a weight of 240 lbs.

---

**👤 You:**
> "If I lift 225 lbs for 3 reps and my 1RM is 275 lbs, what is my RPE?"

**🤖 AI Agent:**
> Lifting 225 lbs for 3 reps with a 275 lbs 1RM results in an estimated RPE of 8.0.

---

**👤 You:**
> "How many reps in reserve is an RPE of 7?"

**🤖 AI Agent:**
> An RPE of 7 is equivalent to 3 reps in reserve.


## ❓ FAQ

**Q: How do I use this to plan my workout?**
You can use `calculate_target_weight` by providing your estimated 1RM, your target RPE, and the number of reps you want to perform to get your target weight.

**Q: What is the difference between RPE and RIR?**
RPE is the Rating of Perceived Exertion, while RIR is Reps in Reserve. You can use `get_rep_reserve_info` to convert between them instantly.

**Q: Can I adjust my weights if I am feeling tired?**
Yes, use `adjust_for_fatigue` to reduce your target weight based on a fatigue factor to ensure you still hit your target RPE.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/rpe-to-weight-converter](https://vinkius.com/en/ai-agent-connect/rpe-to-weight-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RPE to Weight Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rpe-to-weight-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RPE to Weight Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rpe-to-weight-converter": {
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
