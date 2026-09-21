# Creator Sponsorship Rate Card MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/creator-sponsorship-rate-card)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

A specialized pricing engine for influencer marketing campaigns.

## Description
This MCP server provides a professional pricing engine for the creator economy. It translates audience metrics, content complexity, and legal rights into actionable campaign rate cards. Use `calculate_base_rate` to establish foundational costs, `calculate_add_ons` for complexity and exclusivity fees, `generate_package_price` to finalize commercial offers, and `simulate_negotiation` to determine strategic walk-away numbers.


## Available Tools (4)
- **calculate_add_ons**: Quantify extra costs associated with complexity, usage rights, and urgency
- **calculate_base_rate**: Determine the foundational cost of a sponsorship based on audience metrics and platform
- **generate_package_price**: Compile the final commercial offer, including all deliverables and profit margins
- **simulate_negotiation**: Provide walk-away numbers and strategic pricing scenarios


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Creator Sponsorship Rate Card** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the base rate for a YouTube creator with 500,000 followers, 50,000 average views, and a 5% engagement rate."

**🤖 AI Agent:**
> The calculated base rate for this YouTube creator is $2,500.00.

---

**👤 You:**
> "What is the total package price for a campaign with a $1,000 base rate, $500 in add-ons, 3 deliverables, a 20% margin, and 100,000 projected views?"

**🤖 AI Agent:**
> The final package price is $1,800.00, with an effective CPM of $18.00.

---

**👤 You:**
> "Simulate negotiation scenarios for a $5,000 package where the minimum acceptable rate is $4,200, testing 5%, 10%, and 15% discounts."

**🤖 AI Agent:**
> A 5% discount ($4,750) and a 10% discount ($4,500) are successful. A 15% discount ($4,250) is also successful. All scenarios remain above your $4,200 floor.


## ❓ FAQ

**Q: How is the base rate determined?**
The base rate is calculated using `calculate_base_rate` based on audience size, average views, platform type, and engagement rate.

**Q: Can I include exclusivity fees?**
Yes, you can use `calculate_add_ons` to include fees for category exclusivity and usage rights duration.

**Q: How do I calculate the final price for a client?**
Use `generate_package_price` to combine the base rate, add-ons, number of deliverables, and your target profit margin.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/creator-sponsorship-rate-card](https://vinkius.com/en/ai-agent-connect/creator-sponsorship-rate-card)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Creator Sponsorship Rate Card** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `creator-sponsorship-rate-card` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Creator Sponsorship Rate Card** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "creator-sponsorship-rate-card": {
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
