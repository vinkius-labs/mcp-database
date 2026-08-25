# Accelerator Follow-up Metrics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-follow-up-metrics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate follow-up conversion rates, deal velocity, and time compression for accelerator programs.

## Description
This MCP server provides tools to evaluate the effectiveness of accelerator programs following Demo Day. It uses a Follow-up Funnel Model to calculate key performance indicators such as conversion rates from initial meetings to term sheets, deal velocity, and time compression. By accounting for investor types (Angel, VC, Family Office) and deal complexity (Low, Medium, High), it helps program managers optimize investor engagement and accelerate deal closing speeds. Use `calculate_conversion_metrics` to analyze the funnel, `calculate_velocity_and_compression` to measure speed improvements, and `evaluate_investor_engagement` to calibrate expectations based on investor profiles.


## Available Tools (3)
- **calculate_conversion_metrics**: 
- **calculate_velocity_and_compression**: 
- **evaluate_investor_engagement**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Follow-up Metrics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was our conversion efficiency for the last cohort?"

**🤖 AI Agent:**
> The conversion rate for the last cohort was 25%, with a meeting-to-term ratio of 0.15.

---

**👤 You:**
> "How much time did we compress for our high-complexity seed rounds?"

**🤖 AI Agent:**
> For high-complexity rounds, we achieved a time compression of 15 days with a deal velocity of 0.85.

---

**👤 You:**
> "What should be our follow-up frequency for a VC investor after 2 meetings?"

**🤖 AI Agent:**
> For a VC investor after 2 meetings, the expected conversion threshold is 15% and the recommended follow-up frequency is weekly.


## ❓ FAQ

**Q: How do I calculate my follow-up conversion rate?**
You can use the `calculate_conversion_metrics` tool by providing the total number of initial investor meetings, the number of follow-up meetings achieved, and the total term sheets received.

**Q: Can I adjust for different types of investors?**
Yes, the `evaluate_investor_engagement` tool allows you to input the investor type--such as angel, vc, or family_office--to determine expected conversion thresholds and recommended follow-up frequencies.

**Q: How is deal velocity measured?**
Deal velocity is calculated using the `calculate_velocity_and_compression` tool, which takes the time to close, the accelerator's speedup factor, and the deal complexity into account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-follow-up-metrics](https://vinkius.com/ai-agent-connect/accelerator-follow-up-metrics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Follow-up Metrics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-follow-up-metrics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Follow-up Metrics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-follow-up-metrics": {
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
