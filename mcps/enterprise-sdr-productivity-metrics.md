# Enterprise SDR Productivity Metrics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-sdr-productivity-metrics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate SDR efficiency, capacity, and performance benchmarks for enterprise sales teams.

## Description
This MCP server provides specialized analytics for Sales Development Representative (SDR) teams operating in complex enterprise environments. It allows AI agents to calculate critical performance indicators including meetings per SDR, qualification rates, and total team capacity. By using tools like `get_team_productivity_summary` and `calculate_individual_capacity`, managers can assess how ramp time and new hires impact overall output. The engine also evaluates engagement through `analyze_outreach_efficiency` and classifies performance using `get_productivity_benchmarks` to identify if a team is performing at an Elite or Standard level.


## Available Tools (4)
- **calculate_individual_capacity**: Determines the total output potential of the SDR team, adjusted for new hires still in training
- **get_productivity_benchmarks**: Compares current team performance against standardized enterprise tiers
- **get_team_productivity_summary**: Provides a high-level overview of the team's efficiency and output
- **analyze_outreach_efficiency**: Evaluates the relationship between activity volume and meeting generation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise SDR Productivity Metrics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current productivity summary for a team of 10 SDRs with 50 meetings booked and 10 qualified opportunities?"

**🤖 AI Agent:**
> The team has 5.0 meetings per SDR, a 20% qualification rate, and an efficiency score of 0.45.

---

**👤 You:**
> "Calculate the capacity for 5 SDRs where 2 are still ramping for 3 months, with a target of 10 meetings per month."

**🤖 AI Agent:**
> The total team capacity is 42.5 meetings per month, with an effective SDR count of 4.25.

---

**👤 You:**
> "Evaluate the outreach efficiency for 500 activities, 25 meetings, a complexity of 1.5, and messaging efficiency of 1.2."

**🤖 AI Agent:**
> The activity to meeting ratio is 0.05 and the engagement score is 0.18.


## ❓ FAQ

**Q: How does this tool account for new SDRs in training?**
The `calculate_individual_capacity` tool specifically adjusts the total team output by accounting for the productivity lost during the ramp period of new hires.

**Q: Can I compare my team's performance against industry standards?**
Yes, you can use `get_productivity_benchmarks` to classify your team into tiers such as Elite, Standard, or Volume-Driven based on their metrics.

**Q: What metrics are included in the productivity summary?**
The `get_team_productivity_summary` tool provides meetings per SDR, the qualification rate, and a derived efficiency score.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-sdr-productivity-metrics](https://vinkius.com/ai-agent-connect/enterprise-sdr-productivity-metrics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise SDR Productivity Metrics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-sdr-productivity-metrics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise SDR Productivity Metrics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-sdr-productivity-metrics": {
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
