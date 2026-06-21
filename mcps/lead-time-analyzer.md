# Lead Time Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lead-time-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Analyze and decompose supply chain lead times to identify bottlenecks.

## Description
The Lead Time Analyzer is a specialized tool for supply chain professionals. It decomposes total lead time into specific stages, allowing you to distinguish between Value-Added and Non-Value-Added time. By using tools like `analyze_lead_time_composition`, you can identify the primary bottleneck in your process. Additionally, `calculate_reduction_impacts` allows you to simulate a 20% reduction in any stage to see its effect on the total duration, while `evaluate_process_volatility` helps you understand which stages contribute most to process uncertainty.


## Available Tools (3)
- **analyze_lead_time_composition**: Calculates the core metrics of the lead time breakdown
- **calculate_reduction_impacts**: Simulates efficiency gains by optimizing specific stages
- **evaluate_process_volatility**: Determines which stages contribute most to the unpredictability of the total lead time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lead Time Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze my lead time: Order Processing is 2h, Production/Picking is 5h, Transport is 10h, Receiving is 3h, and Inspection is 2h."

**🤖 AI Agent:**
> The total lead time is 22 hours. The bottleneck stage is Transport (10h). Value-Added time is 5h, and Non-Value-Added time is 17h.

---

**👤 You:**
> "What happens to my total lead time if I reduce the Transport stage by 20%?"

**🤖 AI Agent:**
> If you reduce the Transport stage from 10h to 8h, your new total lead time will be 20 hours, resulting in a reduction of 2 hours.

---

**👤 You:**
> "Which stage contributes most to the variability of my process? (Deviations: Order Processing: 0.5, Production/Picking: 1, Transport: 3, Receiving: 0.2, Inspection: 0.1)"

**🤖 AI Agent:**
> The stage contributing most to the process volatility is Transport.


## ❓ FAQ

**Q: How can I identify the main bottleneck in my process?**
Use the `analyze_lead_time_composition` tool. It will return the `bottleneckStage`, which is the stage with the highest duration.

**Q: Can I simulate the impact of reducing a specific process stage?**
Yes, by using `calculate_reduction_impacts`, you can see the projected total lead time if a chosen stage's duration is reduced by 20%.

**Q: How do I measure process uncertainty?**
The `evaluate_process_volatility` tool calculates the variance contribution of each stage, helping you pinpoint which parts of your supply chain are most unpredictable.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lead-time-analyzer](https://vinkius.com/mcp/lead-time-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lead Time Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lead-time-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lead Time Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lead-time-analyzer": {
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
