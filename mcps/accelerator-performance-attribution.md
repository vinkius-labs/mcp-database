# Accelerator Performance Attribution MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-performance-attribution)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Decompose fund performance into selection and coaching effects.

## Description
This MCP server provides analytical tools to attribute venture capital fund performance to specific accelerator drivers. Use `analyze_performance_drivers` to calculate Alpha, Selection, and Coaching effects. Use `calculate_selection_vs_coaching` to determine if success comes from picking winners or making winners. You can also use `get_sector_vintage_benchmark` to retrieve historical baseline data for normalization against specific sectors and years.


## Available Tools (3)
- **calculate_selection_vs_coaching**: Isolates whether the fund's success is due to "picking winners" (Selection) or "making winners" (Coaching)
- **get_sector_vintage_benchmark**: Retrieves the baseline performance for a specific sector and year
- **analyze_performance_drivers**: Calculates core attribution metrics (Alpha, Selection, and Coaching) to determine the accelerator's total impact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Performance Attribution** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the performance drivers for a fund with 25% returns, 40% accelerator deal flow, 15% support value, 10% non-accelerator return in the SaaS sector for 2022."

**🤖 AI Agent:**
> The total Alpha from the accelerator is 15%, with a Selection Effect of 6% and a Coaching Effect of 9%.

---

**👤 You:**
> "Is the fund's success driven more by picking winners or making winners if selection alpha is 5% and coaching alpha is 10%?"

**🤖 AI Agent:**
> The success is driven 33.3% by selection and 66.7% by coaching, with a selection-to-coaching ratio of 0.5.

---

**👤 You:**
> "What was the benchmark return for the Fintech sector in 2021?"

**🤖 AI Agent:**
> The benchmark return for the Fintech sector in 2021 was 12.5%.


## ❓ FAQ

**Q: How does this tool calculate the coaching effect?**
The coaching effect is the portion of alpha remaining after the selection effect (sourcing quality) is accounted for, representing the value added through direct support.

**Q: Can I normalize results by industry?**
Yes, you can use `get_sector_vintage_benchmark` to retrieve baseline performance for specific sectors and years to ensure accurate normalization.

**Q: What is the difference between selection and coaching?**
Selection refers to the ability to identify high-quality deals, while coaching refers to the performance lift provided through hands-on support and resources.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-performance-attribution](https://vinkius.com/ai-agent-connect/accelerator-performance-attribution)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Performance Attribution** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-performance-attribution` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Performance Attribution** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-performance-attribution": {
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
