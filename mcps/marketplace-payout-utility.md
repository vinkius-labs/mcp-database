# Marketplace Payout Utility MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/marketplace-payout-utility)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculates net payouts by deducting marketplace fees from gross sales.

## Description
This MCP server provides essential financial tools for marketplace operations. It allows AI agents to calculate the exact amount a seller should receive using `get_net_payout`, retrieve specific commission rates via `get_fee_percentage`, and verify if a transaction is ready for processing with `validate_transaction_eligibility`. It also provides a full overview of the current fee structure through `list_tier_rates`.


## Available Tools (4)
- **validate_transaction_eligibility**: Checks if a transaction can be processed for payout based on marketplace rules
- **get_fee_percentage**: Retrieves the specific commission rate applicable to a seller or category
- **get_net_payout**: Calculates the final amount a seller receives from a specific sale
- **list_tier_rates**: Provides a summary of all available fee percentages across different tiers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Marketplace Payout Utility** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the net payout for a $100 sale with a premium seller tier?"

**🤖 AI Agent:**
> The net payout for a $100 sale with a premium seller tier is $95.00, after a $5.00 fee.

---

**👤 You:**
> "Is a sale of $50 eligible for payout if it was refunded?"

**🤖 AI Agent:**
> No, the transaction is ineligible for payout because it has been marked as refunded.

---

**👤 You:**
> "What is the commission rate for a standard tier seller in the electronics category?"

**🤖 AI Agent:**
> The commission rate for a standard tier seller in the electronics category is 12%.


## ❓ FAQ

**Q: How is the net payout calculated?**
The net payout is calculated by taking the gross sale price and subtracting the marketplace fee, which is determined by the seller's tier and the product category.

**Q: Can I check if a specific sale is eligible for payout?**
Yes, you can use `validate_transaction_eligibility` to check if a sale meets the requirements for payout, such as checking if it has been refunded.

**Q: How do I see the different fee tiers available?**
You can use the `list_tier_rates` tool to get a summary of all available fee percentages across different seller tiers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/marketplace-payout-utility](https://vinkius.com/en/ai-agent-connect/marketplace-payout-utility)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Marketplace Payout Utility** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `marketplace-payout-utility` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Marketplace Payout Utility** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "marketplace-payout-utility": {
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
