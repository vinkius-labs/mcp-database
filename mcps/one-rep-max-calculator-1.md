# One-Rep Max Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/one-rep-max-calculator-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sports-science](../categories/sports-science.md)

Estimate 1RM strength, training intensity zones, and RPE from submaximal lifts.

## Description
This MCP server provides a deterministic toolset for strength athletes and coaches to estimate one-repetition maximum (1RM) using established physiological models. By inputting weight and repetitions, you can access multiple estimation formulas including Epley, Brzycki, and Lombardi. The server also calculates training intensity zones for various rep ranges and maps lifts to their estimated Rate of Perceived Exertion (RPE). Use `calculate_1rm_metrics` for a full strength profile or `get_rpe_equivalence` to determine how hard a set felt.


## Available Tools (3)
- **calculate_1rm_metrics**: 
- **get_rpe_equivalence**: Maps lift to RPE
- **validate_lift_integrity**: Checks lift integrity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **One-Rep Max Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my 1RM metrics for lifting 100kg for 5 reps."

**🤖 AI Agent:**
> Your estimated 1RM is 112.5kg based on the average of the formulas. Your training intensity zones for 1-5 reps, 6-8 reps, 9-12 reps, and 13-20 reps are 112.5kg, 95kg, 84kg, and 72kg respectively.

---

**👤 You:**
> "What is the RPE for 80lbs for 10 reps?"

**🤖 AI Agent:**
> The estimated RPE for 80lbs for 10 repetitions is 7.5.

---

**👤 You:**
> "Is a lift of 50kg for 15 reps valid for 1RM estimation?"

**🤖 AI Agent:**
> No, the lift is flagged as unrealistic because repetitions exceed 12 for accurate 1RM estimation.


## ❓ FAQ

**Q: How accurate are these 1RM estimates?**
Estimates are most accurate when repetitions are 12 or fewer. For higher rep counts, the `validate_lift_integrity` tool can flag if the estimation may be unreliable.

**Q: Can I use this for both kilograms and pounds?**
Yes, all tools support both 'kg' and 'lbs' units.

**Q: What is RPE?**
RPE stands for Rate of Perceived Exertion. You can use `get_rpe_equivalence` to estimate how much effort a specific weight and repetition count requires on a standard scale.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/one-rep-max-calculator-1](https://vinkius.com/ai-agent-connect/one-rep-max-calculator-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **One-Rep Max Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `one-rep-max-calculator-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **One-Rep Max Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "one-rep-max-calculator-1": {
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
