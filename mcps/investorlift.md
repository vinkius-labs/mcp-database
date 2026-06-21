# InvestorLift MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/investorlift)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Automate real estate deal sourcing via InvestorLift — list marketplace deals, manage your buy box criteria, and message sellers directly from any AI agent.

## Description
Connect your **InvestorLift** account to any AI agent to streamline your real estate investment workflow. Find off-market deals, analyze property data, and communicate with wholesalers through natural language.

### What you can do

- **Marketplace Access** — Browse and filter thousands of real estate deals using `list_deals` by location and price.
- **Deal Analysis** — Get deep insights into specific properties, including pricing and metadata, with `get_deal`.
- **Investment Strategy** — Retrieve and update your `buy_box` criteria to ensure the AI understands your target ROI and preferred locations.
- **Direct Communication** — Use `send_message` to start negotiations or ask questions to sellers immediately.

### How it works

1. Subscribe to this server
2. Enter your InvestorLift API Key
3. Start sourcing and managing real estate deals from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Real Estate Investors** — quickly find deals that match your specific criteria without manual searching
- **Wholesalers & Agents** — analyze market inventory and communicate with sellers directly from your workflow
- **Investment Analysts** — pull property data into your analysis tools via AI conversation


## Available Tools
- **list_deals**: List available deals in the marketplace
- **get_buy_box**: Get your current buy box criteria
- **get_deal**: Get detailed information about a specific deal
- **send_message**: Send a message to a seller regarding a specific deal
- **update_buy_box**: Update your buy box criteria


## 💬 Prompt Examples

Here are some examples of how you can interact with the **InvestorLift** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available deals in Houston, Texas with a maximum price of $300,000."

**🤖 AI Agent:**
> I've found 3 deals in Houston under $300k. One is a 3-bed fixer-upper (ID: 55432) for $245,000. Would you like more details on any of these?

---

**👤 You:**
> "What are my current investment criteria in my buy box?"

**🤖 AI Agent:**
> Your current buy box is set to target Single Family homes in Florida and Georgia with a minimum ROI of 12% and a price range between $150k and $450k.

---

**👤 You:**
> "Send a message to the seller of deal 98765 saying I am interested in a cash offer."

**🤖 AI Agent:**
> Message sent successfully to the seller of deal 98765. I've let them know you're interested in making a cash offer.


## ❓ FAQ

**Q: How can I filter real estate deals by a specific city and price range?**
You can use the `list_deals` tool. Simply provide parameters like `city`, `min_price`, and `max_price` to narrow down the marketplace results to your specific needs.

**Q: Can I update my investment criteria so the AI finds better matches?**
Yes! Use the `update_buy_box` tool to send a JSON object containing your updated criteria. This helps the system align deal discovery with your investment strategy.

**Q: Is it possible to contact a seller directly through the AI?**
Absolutely. Use the `send_message` tool by providing the `deal_id` and your message text. The AI will deliver your inquiry to the seller regarding that specific property.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/investorlift](https://vinkius.com/mcp/investorlift)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **InvestorLift** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `investorlift` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **InvestorLift** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "investorlift": {
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
