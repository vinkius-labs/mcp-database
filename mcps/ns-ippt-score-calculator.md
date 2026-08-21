# NS IPPT Score Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ns-ippt-score-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Deterministic scoring for National Service IPPT, calculating points, tiers, and incentives.

## Description
This MCP server provides a deterministic engine for calculating National Service Individual Physical Proficiency Test (IPPT) scores. It maps physical performance in push-ups, sit-ups, and the 2.4km run to exact points based on age-specific scoring tables. Users can determine their total score, performance tier (Gold, Silver, Pass, or Fail), and eligibility for completion incentives. Use `calculate_ippt_score` to get a full profile or `get_scoring_table` to inspect specific thresholds for an age group.


## Available Tools (3)
- **calculate_ippt_score**: 
- **get_age_group_thresholds**: Lists all supported age groups
- **get_scoring_table**: Retrieves scoring steps for an exercise and age group


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NS IPPT Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my IPPT score for age group 22-27 with 61 push-ups, 50 sit-ups, and a 2.4km run in 540 seconds."

**🤖 AI Agent:**
> Your IPPT results are: Push-up points: 50, Sit-up points: 35, Run points: 50. Your total score is 135, which qualifies for the Gold tier. You are eligible for the incentive.

---

**👤 You:**
> "What is the scoring table for the run for the 28-32 age group?"

**🤖 AI Agent:**
> The scoring steps for the 2.4km run for age group 28-32 are: 540s (50 pts), 570s (45 pts), 600s (40 pts), and so on.

---

**👤 You:**
> "What age groups are supported?"

**🤖 AI Agent:**
> The supported age groups are: 22-27, 28-32, 33-37, 38-42, 43-47, and 48-52.


## ❓ FAQ

**Q: How is the IPPT score calculated?**
The score is calculated by summing points from three stations: push-ups, sit-ups, and a 2.4km run. Each station is scored based on age-specific tables using the `calculate_ippt_score` tool.

**Q: What are the award tiers?**
Performance is categorized into Gold (>=85), Silver (75-84), Pass (51-74), and Fail (<51).

**Q: Can I see the specific points for my age group?**
Yes, you can use the `get_scoring_table` tool to retrieve the specific point distribution for push-ups, sit-ups, or the run for any supported age group.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ns-ippt-score-calculator](https://vinkius.com/ai-agent-connect/ns-ippt-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NS IPPT Score Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ns-ippt-score-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NS IPPT Score Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ns-ippt-score-calculator": {
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
