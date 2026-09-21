# Podcast Sponsorship Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/podcast-sponsorship-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Calculate precise advertising pricing and campaign ROI for podcast sponsorships.

## Description
This MCP server provides specialized tools for podcasters and media agencies to determine advertising costs and audience reach. Use `get_rate_card` to generate pricing for single units, `calculate_projected_reach` to estimate actual listener engagement, and `calculate_package_total` to determine the full investment for entire campaigns. You can also use `compare_scenarios` to evaluate different advertising strategies based on effective CPM.


## Available Tools (4)
- **calculate_package_total**: Determine the full investment required for an entire advertising campaign
- **calculate_projected_reach**: Estimate how many people will actually hear the advertisement
- **compare_scenarios**: Evaluate the cost-efficiency of different advertising strategies
- **get_rate_card**: Generate a standardized pricing document for a single advertisement unit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Podcast Sponsorship Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the rate card for a podcast with 50,000 downloads, a $25 CPM, and 2 ad slots, including a host-read premium of $500."

**🤖 AI Agent:**
> The base price is $1,250. With 2 ad slots and the $500 host-read premium, the total ad price is $3,000, resulting in a per-slot price of $1,500.

---

**👤 You:**
> "What is the projected reach for 100,000 downloads with a 75% completion rate?"

**🤖 AI Agent:**
> The effective reach is 75,000 listeners.

---

**👤 You:**
> "Calculate the total investment for a campaign with 10 episodes, using a rate card of $2,000 per episode, a $1,000 exclusivity fee, and a $500 production fee."

**🤖 AI Agent:**
> The total investment for the campaign is $21,500.


## ❓ FAQ

**Q: How is the advertising price determined?**
Pricing is calculated using the `get_rate_card` tool, which factors in total downloads, the base CPM, the number of ad slots, and any host-read premiums.

**Q: What is effective CPM?**
Effective CPM is the true cost per 1,000 listeners after accounting for all premiums, production fees, and exclusivity costs across the entire campaign.

**Q: Can I compare different campaign strategies?**
Yes, the `compare_scenarios` tool allows you to evaluate multiple configurations to find the best value based on the lowest effective CPM.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/podcast-sponsorship-calculator](https://vinkius.com/en/ai-agent-connect/podcast-sponsorship-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Podcast Sponsorship Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `podcast-sponsorship-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Podcast Sponsorship Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "podcast-sponsorship-calculator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
