# Customer Acquisition Cost Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/customer-acquisition-cost-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Calculate blended CAC, channel-specific costs, and payback periods.

## Description
This MCP server provides a specialized analytical engine for evaluating customer acquisition efficiency. It allows AI agents to calculate the blended CAC by aggregating marketing, sales, and tool overhead. Users can break down costs by specific acquisition paths using `calculate_channel_cac`, determine the speed of financial recovery with `calculate_channel_payback`, and evaluate the performance gap between paid and organic strategies via `compare_paid_vs_organic_efficiency`.


## Available Tools (4)
- **calculate_blended_cac**: Determines the overall efficiency of the customer acquisition engine by calculating the single average cost per customer across all channels
- **calculate_channel_cac**: Breaks down the cost of acquisition by individual channels to identify which acquisition paths are most and least efficient
- **calculate_channel_payback**: Analyzes the financial recovery speed for each acquisition channel based on customer value
- **compare_paid_vs_organic_efficiency**: Evaluates the performance gap between paid and organic acquisition strategies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Customer Acquisition Cost Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our blended CAC if we spent $50,000 on marketing, $30,000 on sales, and $10,000 on tools, acquiring 1,000 customers?"

**🤖 AI Agent:**
> The blended CAC is $90.00.

---

**👤 You:**
> "Calculate the payback period for a channel with a CAC of $50 if the average customer value is $200."

**🤖 AI Agent:**
> The payback period is 0.25 months.

---

**👤 You:**
> "Break down the CAC for these channels: [{'channelName': 'Paid Search', 'customerCount': 100}, {'channelName': 'Organic', 'customerCount': 50}] with a total investment of $15,000."

**🤖 AI Agent:**
> The CAC for Paid Search is $100.00 and the CAC for Organic is $100.00.


## ❓ FAQ

**Q: How is the blended CAC calculated?**
The blended CAC is calculated by summing the total marketing spend, sales salaries, and tools spend, then dividing that total by the total number of new customers acquired.

**Q: Can I compare paid vs organic channels?**
Yes, you can use the `compare_paid_vs_organic_efficiency` tool to find the efficiency ratio between your paid and organic acquisition channels.

**Q: What is included in the total investment?**
The total investment includes direct marketing spend, sales department salaries, and the cost of software tools used for marketing and sales.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/customer-acquisition-cost-engine](https://vinkius.com/en/ai-agent-connect/customer-acquisition-cost-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Customer Acquisition Cost Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `customer-acquisition-cost-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Customer Acquisition Cost Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "customer-acquisition-cost-engine": {
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
