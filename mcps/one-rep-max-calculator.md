# One Rep Max Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/one-rep-max-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fitness](../categories/fitness.md)

Estimate 1RM using multiple models and generate structured warm-up routines.

## Description
This MCP server provides advanced strength estimation tools for lifters. Use `estimate_one_rep_max` to predict your maximum lift based on submaximal sets using Epley, Brzycki, Lander, Lombardi, and O'Conner models. You can also use `generate_warmup_routine` to create progressive warm-up sets from 40% to 80% intensity, or `lookup_strength_standards` to find benchmarks for squat, bench press, deadlift, and overhead press (OHP).


## Available Tools (3)
- **lookup_strength_standards**: Lookup standardized strength benchmarks
- **estimate_one_rep_max**: Estimate 1RM using multiple formulas
- **generate_warmup_routine**: Generate a structured warmup routine


## 💬 Prompt Examples

Here are some examples of how you can interact with the **One Rep Max Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my 1RM for 100kg at 5 reps."

**🤖 AI Agent:**
> Your average estimated 1RM is 114.6 kg. The intensity table ranges from 100% (114.6 kg) down to 50% (57.3 kg).

---

**👤 You:**
> "Generate a warm-up routine for a 300 lb target 1RM."

**🤖 AI Agent:**
> Your warm-up routine includes sets at 120 lbs, 150 lbs, 180 lbs, 210 lbs, and 240 lbs with increasing rest intervals.

---

**👤 You:**
> "What is the strength standard for a 90kg male doing a deadlift?"

**🤖 AI Agent:**
> The benchmark for an intermediate lifter in the 90kg weight class is 165 kg.


## ❓ FAQ

**Q: How accurate are the 1RM estimates?**
The tool averages five different mathematical models to provide a reliable prediction based on your submaximal performance.

**Q: What lifting movements are supported?**
You can look up standards for squat, bench press, deadlift, and overhead press (OHP).

**Q: Can I generate a warm-up plan?**
Yes, by providing your target 1RM, the tool generates five progressive sets from 40% to 80% intensity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/one-rep-max-calculator](https://vinkius.com/mcp/one-rep-max-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **One Rep Max Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `one-rep-max-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **One Rep Max Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "one-rep-max-calculator": {
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
