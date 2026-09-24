# Resort Fee Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/resort-fee-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate total resort fee liabilities based on nightly rates and stay duration.

## Description
This MCP server provides precise tools for hospitality management and guest billing. It allows AI agents to calculate total resort fee liabilities using `calculate_total_fees`, verify if a stay meets minimum requirements via `validate_stay_eligibility`, look up specific rates with `get_fee_tier_details`, and generate detailed summaries using `summarize_fee_breakdown`.


## Available Tools (4)
- **calculate_total_fees**: Calculates the total resort fee for a specific stay
- **get_fee_tier_details**: Retrieves the specific fee amount based on the tier of the resort
- **summarize_fee_breakdown**: Provides a detailed breakdown of how the total fee was accumulated
- **validate_stay_eligibility**: Determines if a given stay length is eligible for resort fee application


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Resort Fee Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total resort fee for a 3-night stay with a $50 nightly fee?"

**🤖 AI Agent:**
> The total resort fee for a 3-night stay at $50 per night is $150.

---

**👤 You:**
> "Is a 0-night stay eligible for resort fees?"

**🤖 AI Agent:**
> No, a stay must be at least one night to be eligible for resort fees.

---

**👤 You:**
> "How much is the nightly fee for a Luxury tier resort?"

**🤖 AI Agent:**
> The nightly fee for the Luxury tier is $100.


## ❓ FAQ

**Q: How do I calculate the total cost for my stay?**
You can use the `calculate_total_fees` tool by providing the nightly fee and the number of nights stayed.

**Q: Can I check if my stay is eligible for resort fees?**
Yes, use the `validate_stay_eligibility` tool to check if the stay duration meets the minimum requirement.

**Q: What are the different resort tiers available?**
You can use `get_fee_tier_details` to retrieve rates for Luxury, Standard, or Budget tiers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/resort-fee-calculator](https://vinkius.com/en/ai-agent-connect/resort-fee-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Resort Fee Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `resort-fee-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Resort Fee Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "resort-fee-calculator": {
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
