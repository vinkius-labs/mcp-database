# Accelerator Selection Funnel Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-selection-funnel-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Analyze recruitment efficiency and identify friction points in accelerator selection processes.

## Description
This MCP server provides deep analytical insights into the accelerator recruitment lifecycle. It allows AI agents to calculate stage conversion rates, pinpoint specific drop-off reasons, and suggest actionable process improvements. By using tools like `analyze_funnel_conversions` and `identify_dropoff_patterns`, you can identify bottlenecks and optimize the selection flow. The `detect_optimization_opportunities` tool helps mitigate risks like timing lags, while `get_candidate_health_report` provides a real-time overview of applicant quality and attrition risk.


## Available Tools (4)
- **get_candidate_health_report**: Provide a high-level overview of the quality and velocity of the current applicant pool
- **identify_dropoff_patterns**: Optionally filter by a specific reason.

Pinpoint exactly why and where candidates are leaving the funnel
- **analyze_funnel_conversions**: You can optionally include quality weighting.

Calculate the percentage of candidates progressing through every stage of the recruitment process
- **detect_optimization_opportunities**: Suggest actionable improvements to the accelerator's process based on funnel performance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Selection Funnel Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the conversion rates for my current application data."

**🤖 AI Agent:**
> The conversion rate from Application to Initial Screening is 45%, and from Initial Screening to Interview Invite is 30%.

---

**👤 You:**
> "Why are candidates dropping off after the interview stage?"

**🤖 AI Agent:**
> The primary reason for drop-off after interviews is 'declined_offer', accounting for 15% of total losses.

---

**👤 You:**
> "Give me a health report for the current applicant pool."

**🤖 AI Agent:**
> The current pool has an average quality score of 82/100 and an average lead time of 5 days. The attrition risk level is low.


## ❓ FAQ

**Q: How can I identify where I am losing candidates?**
You can use the `identify_dropoff_patterns` tool to see exactly where and why candidates are leaving your funnel.

**Q: Can I weigh conversion rates by candidate quality?**
Yes, the `analyze_funnel_conversions` tool includes an optional parameter to weigh conversion rates based on application quality scores.

**Q: How do I know if my selection process is too slow?**
The `detect_optimization_opportunities` tool flags timing lags that exceed standard windows, helping you prevent candidate drop-off.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-selection-funnel-analyzer](https://vinkius.com/ai-agent-connect/accelerator-selection-funnel-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Selection Funnel Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-selection-funnel-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Selection Funnel Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-selection-funnel-analyzer": {
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
