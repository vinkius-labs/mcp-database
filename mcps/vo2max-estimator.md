# VO2max Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vo2max-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Estimate aerobic capacity using Cooper, Rockport, Step, and YMCA Bike protocols.

## Description
This MCP server provides specialized tools to estimate VO2max (maximal oxygen uptake) through four standardized physical fitness protocols: `calculate_cooper` for the 12-minute run, `calculate_rockport` for the one-mile walk test, `calculate_step_test` for cardiovascular recovery analysis, and `calculate_ymca_bike` for steady-state cycling assessments. Each tool calculates oxygen uptake in ml/kg/min and provides an ACSM fitness classification based on age and sex.


## Available Tools (4)
- **calculate_rockport**: Estimate VO2max using the Rockport Walk Test
- **calculate_step_test**: Estimate VO2max using the Step Test
- **calculate_ymca_bike**: Estimate VO2max using the YMCA Bike Test
- **calculate_cooper**: Estimate VO2max using the Cooper 12-minute run test


## 💬 Prompt Examples

Here are some examples of how you can interact with the **VO2max Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much VO2max did I achieve in my 12-minute run of 2500 meters, assuming I am a 25 year old male?"

**🤖 AI Agent:**
> Your estimated VO2max is 48.5 ml/kg/min, which falls into the Excellent category for a 25-year-old male.

---

**👤 You:**
> "Calculate my VO2max using the Rockport Walk Test: 15 minutes for one mile, heart rate of 140 bpm, weight 75kg, age 30, female."

**🤖 AI Agent:**
> Your estimated VO2max is 38.2 ml/kg/min, which falls into the Good category for a 30-year-old female.

---

**👤 You:**
> "What is my fitness level based on a Step Test with a recovery heart rate of 110 bpm and baseline of 70 bpm for a 40 year old male?"

**🤖 AI Agent:**
> Your estimated VO2max is 35.4 ml/kg/min, which falls into the Fair category for a 40-year-old male.


## ❓ FAQ

**Q: What is the Cooper Test?**
The Cooper Test estimates VO2max by measuring the distance covered during a 12-minute run using the `calculate_cooper` tool.

**Q: How do I use the Rockport Walk Test?**
Use `calculate_rockport` by providing your walking time for one mile, final heart rate, weight, age, and sex.

**Q: Does the server provide fitness classifications?**
Yes, all tools return an ACSM-standardized classification (e.g., Excellent, Good, Fair, or Poor) based on your age and sex.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vo2max-estimator](https://vinkius.com/mcp/vo2max-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **VO2max Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vo2max-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **VO2max Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vo2max-estimator": {
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
