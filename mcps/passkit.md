# PassKit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/passkit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Create digital passes for Apple Wallet and Google Pay with loyalty cards, coupons, and event tickets that update in real time.

## Description
Connect your **PassKit** account to any AI agent and take full control of your digital wallet orchestration through natural conversation. PassKit is the premier platform for creating and managing cards for Apple Wallet and Google Wallet, and this integration allows you to issue loyalty cards, event tickets, and boarding passes directly from your chat interface.

### What you can do

- **Membership & Loyalty Orchestration** — Enroll and manage loyalty program members programmatically and retrieve detailed tier metadata to ensure your customer data is always synchronized.
- **Event Ticket Lifecycle Management** — Issue digital event tickets and monitor usage statuses directly from the AI interface to drive better attendee engagement.
- **Boarding Pass & Flight Intelligence** — Create and manage flight boarding passes via natural language to maintain a clear overview of passenger travel itineraries.
- **Coupon & Campaign Control** — Create and manage digital coupons to ensure your promotional campaigns are always optimized using simple AI commands.
- **Operational Monitoring** — Track system responses and manage branding assets (images) to ensure your pass designs are always high-fidelity.

### How it works

1. Subscribe to this server
2. Enter your PassKit Long-Lived API Token from your dashboard settings
3. Specify your regional Base URL (e.g., https://api.pub1.passkit.io for EU/Asia)
4. Start managing your digital passes from Claude, Cursor, or any MCP-compatible client

No more manual pass generation or switching between wallet dashboards. Your AI acts as a dedicated digital wallet coordinator or customer engagement lead.

### Who is this for?

- **Retailers & Marketers** — quickly retrieve loyalty summaries and monitor program growth without switching apps.
- **Event Organizers** — automate the issuance of digital tickets and track entry metrics via natural conversation.
- **Travel Providers** — streamline the retrieval of flight metadata and monitor passenger check-ins directly within the chat.


## Available Tools
- **create_coupon**: Create a new digital coupon
- **create_flight**: Create a new flight
- **enroll_member**: Enroll a new member
- **get_member_details**: Get member details
- **get_pass_template**: Get details for a pass template
- **get_event_ticket**: Get details for an issued ticket
- **issue_boarding_pass**: Issue a boarding pass
- **issue_event_ticket**: Issue a new event ticket
- **list_branding_images**: List uploaded branding images
- **get_coupon_details**: Get details for a specific coupon pass
- **update_member**: Update member data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PassKit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my branding images in PassKit."

**🤖 AI Agent:**
> I've retrieved your assets. You have 5 active images including your company logo and several promotional banners. Would you like to use any of these in a new pass design?

---

**👤 You:**
> "Issue a new digital loyalty card for member sarah.chen@example.com with 500 welcome points."

**🤖 AI Agent:**
> Loyalty card issued successfully for sarah.chen@example.com. Member ID: MBR-29847. Tier: Silver. Welcome points: 500 credited. The digital pass has been generated and an enrollment email sent with Apple Wallet and Google Pay installation links. The pass includes a personalized barcode for in-store scanning.

---

**👤 You:**
> "Create a promotional coupon pass for our 25% off summer sale valid until August 31st."

**🤖 AI Agent:**
> Coupon pass created successfully (ID: CPN-8421). Discount: 25% off entire purchase. Valid: Now through August 31, 2025. The pass features your brand colors and summer campaign artwork. Distribution URL generated for email campaigns and social media sharing. Supports both Apple Wallet and Google Pay. Redemption limit set to single use per customer.


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific loyalty member by their ID?**
Yes! Use the `get_member` tool with the Member ID. Your agent will respond with complete metadata, including current points, tier status, and enrollment date in seconds.

**Q: How do I find my PassKit Long-Lived API Token?**
Log in to the [**PassKit Portal**](https://portal.passkit.com/), navigate to **Settings** > **Integrations**, and you will find your unique secret token under the API Credentials section.

**Q: Does this work with both Apple and Google Wallets?**
Absolutely. PassKit acts as a unified hub, allowing the AI to orchestrate digital passes that are cross-compatible with both major mobile wallet ecosystems.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/passkit](https://vinkius.com/mcp/passkit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PassKit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `passkit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PassKit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "passkit": {
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
