# Accelerator Alumni Network Value MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-alumni-network-value)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Quantifies the economic and strategic value of an accelerator's alumni network.

## Description
This MCP server provides advanced network effect modeling to quantify the value of an accelerator's ecosystem. It calculates three core dimensions: Network Density, which measures community interconnectedness using `get_network_density`; Referral Value, which quantifies financial impact via `get_referral_economic_value`; and Brand Equity, which estimates reputational prestige through `get_brand_equity_value`. It is designed to help accelerator managers understand the compounding benefits of alumni engagement and successful exits.


## Available Tools (3)
- **get_brand_equity_value**: Estimates the prestige and reputational value of the accelerator based on alumni success
- **get_referral_economic_value**: Quantifies the financial impact generated through alumni-to-alumni referrals and capital flow
- **get_network_density**: Determines how interconnected and active the alumni community is


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Alumni Network Value** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the network density for 50 alumni companies with 20% active mentors?"

**🤖 AI Agent:**
> The network density score is 10.0, which indicates a Medium engagement level.

---

**👤 You:**
> "Calculate the referral economic value for 100 companies that raised $50M with a 5% referral rate."

**🤖 AI Agent:**
> The referral value is $25,000,000 with a capital velocity of 250,000.

---

**👤 You:**
> "What is the brand equity for an accelerator with 10 exits, 100 companies, and a density score of 15?"

**🤖 AI Agent:**
> The brand equity score is 150, placing the accelerator in the Established reputation tier.


## ❓ FAQ

**Q: What is Network Density?**
Network Density represents the strength and interconnectedness of the alumni ecosystem, calculated using the `get_network_density` tool.

**Q: How is referral value calculated?**
Referral value is determined by the `get_referral_economic_value` tool, which uses total funding raised and the referral rate to quantify financial impact.

**Q: Can I estimate my brand prestige?**
Yes, you can estimate prestige using `get_brand_equity_value`, which factors in completed exits and network density.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-alumni-network-value](https://vinkius.com/ai-agent-connect/accelerator-alumni-network-value)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Alumni Network Value** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-alumni-network-value` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Alumni Network Value** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-alumni-network-value": {
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
