# Hypertrophy Rep Range Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hypertrophy-rep-range-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track and optimize muscle hypertrophy by monitoring training volume, RIR targets, and effective stimulus.

## Description
The Hypertrophy Rep Range Calculator is a specialized tool for lifters looking to optimize their training using the principles of MEV (Minimum Effective Volume), MAV (Maximum Adaptive Volume), and MRV (Maximum Recoverable Volume). By tracking your weekly sets, RIR (Reps in Reserve), and mesocycle phases, you can ensure you are providing enough stimulus for growth without exceeding your recovery capacity.

With this MCP server, you can use tools like `calculate_group_volume` to sum up your weekly workload, `evaluate_volume_adequacy` to check if you are hitting your target ranges, and `compute_effective_volume` to see how much of your training is actually driving hypertrophy based on intensity. It's the perfect companion for managing accumulation, intensification, and deload phases.


## Available Tools (4)
- **compute_effective_volume**: Compute effective stimulus volume
- **calculate_group_volume**: Calculate total weekly sets per muscle group
- **get_rir_targets**: Get recommended RIR range for a training phase
- **evaluate_volume_adequacy**: Evaluate if weekly volume is adequate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hypertrophy Rep Range Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my total weekly sets for Bench Press (3 sets) and Overhead Press (4 sets) for Chest."

**🤖 AI Agent:**
> Total weekly sets for Chest: 7

---

**👤 You:**
> "Is my current volume of 10 sets for Quads adequate if my MEV is 8 and MRV is 15?"

**🤖 AI Agent:**
> Your volume for Quads is Optimal.

---

**👤 You:**
> "What RIR should I target during an Intensification phase?"

**🤖 AI Agent:**
> During the Intensification phase, your target RIR range is 0 to 2.


## ❓ FAQ

**Q: How does the calculator determine if my volume is adequate?**
The `evaluate_volume_adequacy` tool compares your actual weekly sets against your established MEV and MRV thresholds. It will flag if you are 'Under' (below MEV), 'Optimal' (within MAV), or 'Over' (exceeding MRV) for each muscle group.

**Q: What is 'Effective Volume' in this tool?**
Effective volume is a metric that weights your sets based on intensity. Using `compute_effective_volume`, the tool excludes any sets performed with an RIR (Reps in Reserve) greater than 3, as these are considered to provide insufficient stimulus for hypertrophy.

**Q: Can I use this to plan my mesocycle phases?**
Yes. You can use `get_rir_targets` to find the recommended RIR range for your current phase, whether you are in Accumulation, Intensification, or Deload.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hypertrophy-rep-range-calculator](https://vinkius.com/mcp/hypertrophy-rep-range-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hypertrophy Rep Range Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hypertrophy-rep-range-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hypertrophy Rep Range Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hypertrophy-rep-range-calculator": {
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
