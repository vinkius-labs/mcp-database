# Customer Rating Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/customer-rating-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Calculate statistical summaries, distributions, and ranges for star ratings.

## Description
This MCP server provides tools to analyze customer feedback through star ratings. Use `calculate_rating_metrics` to get the average, total count, and a rounded display rating from a list of ratings. You can also use `get_rating_distribution` to see the frequency of each star level, `get_rating_summary_by_range` to count ratings within specific satisfaction tiers, or `validate_rating_input` to verify if a single rating is valid.


## Available Tools (4)
- **calculate_rating_metrics**: 
- **get_rating_distribution**: 
- **get_rating_summary_by_range**: 
- **validate_rating_input**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Customer Rating Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the statistical summary for these ratings: [5, 4, 5, 3, 5, 2, 4, 5]?"

**🤖 AI Agent:**
> The average rating is 4.125, with a total of 8 ratings. The display rating is 4.

---

**👤 You:**
> "How many ratings are in the high satisfaction range (4 to 5 stars) for [5, 4, 3, 2, 5, 1, 4]?"

**🤖 AI Agent:**
> There are 3 ratings in the 4 to 5 star range.

---

**👤 You:**
> "Show me the distribution of these ratings: [1, 1, 2, 3, 4, 5, 5, 5]?"

**🤖 AI Agent:**
> The distribution is: 1 star: 2, 2 stars: 1, 3 stars: 1, 4 stars: 1, 5 stars: 3.


## ❓ FAQ

**Q: What kind of data can I analyze?**
You can analyze arrays of integer star ratings ranging from 1 to 5 using `calculate_rating_metrics` and other specialized tools.

**Q: How do I check if a rating is valid?**
Use the `validate_rating_input` tool to confirm if a specific integer falls within the required 1 to 5 star range.

**Q: Can I see how many people gave 5 stars?**
Yes, use `get_rating_distribution` to receive an object showing the count for every star level from 1 to 5.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/customer-rating-analytics](https://vinkius.com/en/ai-agent-connect/customer-rating-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Customer Rating Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `customer-rating-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Customer Rating Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "customer-rating-analytics": {
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
