# Brunch Cost & Instagram ROI Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/brunch-cost-instagram-roi-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate the economic efficiency and social ROI of your café visits.

## Description
This MCP server provides tools for content creators to evaluate the financial and social value of dining experiences. Use `calculate_brunch_metrics` to determine your cost per photo and Instagram ROI based on brunch expenditure, wait times, and expected engagement. You can also use `get_location_vibe` to understand the atmosphere of different districts or `compare_venue_efficiency` to decide which café offers the best value for your content creation.


## Available Tools (3)
- **get_location_vibe**: Answers what general atmosphere or density a specific café location represents
- **calculate_brunch_metrics**: Provides a full economic breakdown of a specific brunch visit, including photo efficiency and social ROI
- **compare_venue_efficiency**: Allows a user to compare the efficiency of two different brunch experiences


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brunch Cost & Instagram ROI Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I spent 45 SGD at a café in CBD. The photo worthiness is 8, I waited 15 minutes, and I expect 200 likes. What is my ROI?"

**🤖 AI Agent:**
> Your cost per photo is 5.63 SGD, your total cost is 75.00 SGD, and your Instagram ROI is 1.33.

---

**👤 You:**
> "What is the vibe of Tiong Bahru?"

**🤖 AI Agent:**
> Tiong Bahru is a trendy, heritage-meets-modern district with medium to high costs.

---

**👤 You:**
> "Calculate metrics for a 35 SGD brunch in Haji Lane with a photo score of 7, 10 min wait, and 150 expected likes."

**🤖 AI Agent:**
> Your cost per photo is 5.00 SGD, your total cost is 65.00 SGD, and your Instagram ROI is 1.15.


## ❓ FAQ

**Q: How is the Instagram ROI calculated?**
The ROI is calculated by multiplying your expected likes by a social value of 0.5 SGD and dividing that by your total cost (brunch cost plus time cost).

**Q: What is included in the total cost?**
The total cost includes the direct price of the brunch and the opportunity cost of your time spent waiting and eating.

**Q: Can I compare two different cafés?**
Yes, you can use the `compare_venue_efficiency` tool to see which venue provides a higher Instagram ROI.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/brunch-cost-instagram-roi-calculator](https://vinkius.com/ai-agent-connect/brunch-cost-instagram-roi-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Brunch Cost & Instagram ROI Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `brunch-cost-instagram-roi-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Brunch Cost & Instagram ROI Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "brunch-cost-instagram-roi-calculator": {
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
