# Attribution Model Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/attribution-model-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-analytics](../categories/marketing-analytics.md)

Compare 5 attribution models (First Touch, Last Touch, Linear, etc.) to quantify revenue delta across all marketing channels.

## Description
**The Challenge of Credit Allocation:** When a customer completes a purchase, how do you accurately assign credit for that revenue? Did the initial social media ad (First Touch) or the final email reminder (Last Touch) drive the sale? Traditional models often fail to capture the true value contribution across an entire customer journey. The simple answer is: it's complicated.


## Available Tools
- **calculate_attribution_shares**: Returns individual channel shares with percentage weights.

Calculate proportional revenue share credit for each touchpoint using a specific attribution model
- **fetch_conversion_metrics**: Reconciles multiple sales records linked by conversionId.

Retrieve the total revenue value and currency for a specific conversion event
- **calculate_attribution_delta**: Use this to identify which models over- or under-credit specific channels.

Compare attribution share results across multiple models to determine revenue discrepancy for a target channel
- **get_customer_journey**: Use this to establish input data for attribution model calculations.

Retrieve the chronologically ordered touchpoint sequence for a customer leading up to a conversion event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Attribution Model Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to compare how First Touch and Last Touch allocate revenue for customer CUST-123 on 2024-05-15. Start by getting the journey data."

**🤖 AI Agent:**
> First, I will call `get_customer_journey` to establish the touchpoint sequence. Then, using that sequence and the total revenue from `fetch_conversion_metrics`, I will run `calculate_attribution_shares` for both models. Finally, I'll use `calculate_attribution_delta` to quantify the difference.

---

**👤 You:**
> "Analyze the attribution shares for a high-value conversion ID CONV-900. Use all five models and target 'Google Paid Search' to see its delta."

**🤖 AI Agent:**
> I will use `fetch_conversion_metrics` first. Then, I will call `calculate_attribution_shares` five times (once for each model type) using the journey data and total revenue. With all results compiled, I will pass them to `calculate_attribution_delta`, specifying 'Google Paid Search' as the target channel.

---

**👤 You:**
> "I have the journey data and total revenue. Please calculate the attribution shares for all five models for this customer, focusing on understanding the relative contribution of Email Newsletter."

**🤖 AI Agent:**
> I will call `calculate_attribution_shares` multiple times using the full list of models: 'First Touch', 'Last Touch', 'Linear', 'Time Decay', and 'Position-Based'. This provides a complete picture before running any delta comparison.


## ❓ FAQ

**Q: What is the necessary input data to start an attribution comparison?**
You must first use the `get_customer_journey` tool, providing a customer ID and conversion date. This establishes the ordered sequence of touchpoints needed for all subsequent calculations.

**Q: How do I get the financial value used as a baseline for attribution?**
Use `fetch_conversion_metrics` with the specific conversion ID. This tool retrieves the total revenue amount, which serves as the single, absolute figure that all five attribution models will proportionally divide.

**Q: After calculating shares for multiple models, how do I find out which model is most biased?**
The `calculate_attribution_delta` tool takes the full results from all share calculations (via `calculate_attribution_shares`) and compares them. It quantifies the revenue gain or loss for a specific channel across models, highlighting discrepancies.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/attribution-model-comparator](https://vinkius.com/mcp/attribution-model-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Attribution Model Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `attribution-model-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Attribution Model Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "attribution-model-comparator": {
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
