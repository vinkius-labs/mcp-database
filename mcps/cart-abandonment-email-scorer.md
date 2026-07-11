# Cart Abandonment Email Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cart-abandonment-email-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Analyze email copy for urgency, scarcity, and incentive clarity.

## Description
This MCP server provides linguistic analysis for cart-recovery emails. Use `analyze_urgency` to detect scarcity triggers like 'last chance' and `evaluate_incentive` to assess how clearly discounts or promotional offers are communicated to your customers.


## Available Tools (2)
- **evaluate_incentive**: Evaluate how clearly a discount or promotional offer is communicated
- **analyze_urgency**: Analyze the presence of scarcity and urgency triggers in an email


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cart Abandonment Email Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this email: 'Don't forget your items! Use code SAVE10 for a discount.'"

**🤖 AI Agent:**
> The `analyze_urgency` tool reports low strength. The `evaluate_incentive` tool identifies an explicit offer: 'SAVE10'.

---

**👤 You:**
> "Check the urgency in this subject line: 'Hurry! Only a few left in your cart!'"

**🤖 AI Agent:**
> The `analyze_urgency` tool detects high strength with triggers: 'Hurry!', 'Only a few left'.

---

**👤 You:**
> "Is the discount clear in: 'A special surprise is waiting for you at checkout.'"

**🤖 AI Agent:**
> The `evaluate_incentive` tool returns a clarity level of 'vague' because no specific value or discount amount is mentioned.


## ❓ FAQ

**Q: What does the urgency analysis detect?**
The `analyze_urgency` tool identifies time-sensitive language such as 'expiring soon' or 'limited stock' and rates the intensity of these triggers.

**Q: How is incentive clarity measured?**
The `evaluate_incentive` tool checks if your offer, such as '15% off', is explicitly stated or remains too vague for the customer to understand.

**Q: Can I use this for non-English emails?**
Currently, the linguistic patterns are optimized for English text to ensure accurate scoring of urgency and incentive clarity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cart-abandonment-email-scorer](https://vinkius.com/mcp/cart-abandonment-email-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cart Abandonment Email Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cart-abandonment-email-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cart Abandonment Email Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cart-abandonment-email-scorer": {
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
