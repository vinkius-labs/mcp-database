# Upsell & Cross-sell Copy Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/upsell-cross-sell-copy-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Analyze up-sell and cross-sell copy for economic clarity, product relevance, and linguistic friction.

## Description
The Upsell & Cross-sell Copy Analyzer evaluates marketing text to ensure high conversion rates. It uses `analyze_offer_economics` to check for value-delta clarity and anchor comparisons, `analyze_purchase_relevance` to measure the connection between existing purchases and new offers, and `audit_copy_sentiment` to identify friction words and assess CTA urgency-to-value balance.


## Available Tools (3)
- **analyze_offer_economics**: Determines if the economic benefits and comparison points of an offer are clearly communicated
- **analyze_purchase_relevance**: Evaluates how well the copy links the new offer to the consumer's previous purchase history
- **audit_copy_sentiment**: Identifies linguistic resistance and assesses the balance of the Call-to-Action


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Upsell & Cross-sell Copy Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this up-sell text: 'Upgrade your basic plan to premium for just $10 more and get unlimited access!' using analyze_offer_economics with originalPrice 50 and newPrice 60."

**🤖 AI Agent:**
> The analysis shows a clear value-delta of $10. The price difference is specific, and the anchor comparison is present.

---

**👤 You:**
> "Check this copy for friction: 'Our complex setup process is worth the wait. Click here to buy now!'"

**🤖 AI Agent:**
> The `audit_copy_sentiment` tool identified 2 friction words ('complex', 'wait') and flagged the CTA as imbalanced due to high urgency without sufficient value reinforcement.

---

**👤 You:**
> "Evaluate relevance: 'Since you bought a Coffee Maker, you will love our Premium Bean Subscription.' using analyze_purchase_relevance for Coffee Maker."

**🤖 AI Agent:**
> The tool found a high connection strength with keywords like 'since' and 'love', indicating strong linguistic bridging between the products.


## ❓ FAQ

**Q: How does the tool evaluate economic clarity?**
By using `analyze_offer_economics`, the tool checks if the text explicitly mentions the price difference (value-delta) and uses specific numbers rather than vague terms.

**Q: Can it identify words that cause buyer hesitation?**
Yes, the `audit_copy_sentiment` tool counts friction words like 'difficult' or 'complex' that might induce psychological resistance.

**Q: How is product relevance measured?**
The `analyze_purchase_relevance` tool looks for linguistic bridges that connect the consumer's original purchase to the new recommendation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/upsell-cross-sell-copy-analyzer](https://vinkius.com/mcp/upsell-cross-sell-copy-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Upsell & Cross-sell Copy Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `upsell-cross-sell-copy-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Upsell & Cross-sell Copy Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "upsell-cross-sell-copy-analyzer": {
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
