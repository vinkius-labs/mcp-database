# Patreon Tiers & Members MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/patreon-tiers-members)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [billing-subscriptions](../categories/billing-subscriptions.md)

Patreon tier and member detail APIs as an MCP: campaign tiers with amounts/benefits, member shipping addresses and tier history, user profiles, funding goals — official API v2 JSON:API (complementary to the Patreon creator subscriptions MCP).

## Description
**Patreon tier and member detail APIs** (API v2, JSON:API) as a single MCP server — the deeper membership layer complementing the campaigns/members/posts companion.

### What you can do
- **Campaign tiers** — full tier objects: amount_cents, titles, descriptions, patron counts, linked benefits
- **Member addresses** — shipping addresses for physical rewards (creator scope)
- **Member tier history** — currently entitled tiers, pledge history and lifetime support per member
- **User profiles** — public profiles of ANY Patreon user by id (name, vanity, about, image)
- **Funding goals** — campaign milestone goals with completion percentages

### Authentication
Same OAuth2 access token as the Patreon creator subscriptions MCP — create an app at patreon.com/portal, get the creator's authorization code, and paste the Bearer token. JSON:API responses use `data`, `included`, `relationships` — fields must be explicitly requested with URL-encoded brackets (`fields%5Btier%5D=amount_cents,title`).

### Who is this for?
Creator analytics, reward fulfilment, patron CRM tools and AI agents that need the deep membership layer of Patreon campaigns.


## Available Tools (6)
- **get_member_address**: Get a member's shipping address (for physical rewards fulfilment)
- **get_user_by_vanity**: g. patreon.com/anker) to a user id — search-free: GET /user/{id} after discovery via campaign includes. Note: Patreon v2 has no vanity search; use get_campaign_tiers include=creator to find creator user ids.

Find a Patreon user id by their vanity URL slug (www.patreon.com/{vanity})
- **get_campaign_tiers**: campaign_id from the companion patreon-creator-subscriptions-mcp list_campaigns.

Get all membership tiers of a campaign with amounts, titles and benefits
- **get_user_profile**: Different from get_identity (the token owner): this works for ANY user id.

Get any Patreon user profile by id (public fields: name, vanity, image, about)
- **get_campaign_goals**: Goals are a strong engagement signal for content planning.

Get the funding goals of a campaign (target amounts and progress)
- **get_member_tiers_history**: Get the entitled tiers and payment history context of a member


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Patreon Tiers & Members** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all membership tiers of my campaign with their benefits"

**🤖 AI Agent:**
> 🎯 **Campaign tiers (JSON:API included=tiers)**

1. **Starter** — $3/month: early access to videos, patron-only feed
2. **Supporter** — $10/month: + exclusive blog, Discord role
3. **Insider** — $25/month: + monthly Q&A, name in credits

Patron counts and benefit lists included. Want the shipping addresses of Insider members?

---

**👤 You:**
> "Get the shipping address of member 123-456-789 for the reward shipment"

**🤖 AI Agent:**
> 📦 **Member shipping address (creator scope)**

Member: 123-456-789, patron status: active_patron
Entitled amount: $25/mo

Address:
- Addressee: John Doe
- Line 1: 123 Main St
- City: Austin, TX 78701, US

Creator scope required — addresses are only exposed to the campaign owner.

---

**👤 You:**
> "How close is my campaign to its funding goals?"

**🤖 AI Agent:**
> 🎯 **Campaign goals progress**

1. First milestone — $1,000/mo: ✅ 145% completed
2. Studio upgrade — $3,000/mo: 🔶 48% completed

Goals are pulled from included=goals with completion percentages. Want the tier breakdown driving the progress?


## ❓ FAQ

**Q: Do I need the same access token as the Patreon creator subscriptions MCP?**
Yes — same OAuth2 Bearer token, same scopes. The difference is the endpoint layer: that MCP covers campaigns/members/posts/identity/webhooks CRUD; this one covers the deeper tier, address, user profile and goals layer with no tool overlap.

**Q: Why are fields URL-encoded with brackets?**
Patreon API v2 uses the JSON:API specification: fields[member]=full_name is the standard sparse fieldset syntax, and brackets must be URL-encoded (fields%5Bmember%5D=full_name). The MCP handles the encoding automatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/patreon-tiers-members](https://vinkius.com/ai-agent-connect/patreon-tiers-members)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Patreon Tiers & Members** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `patreon-tiers-members` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Patreon Tiers & Members** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "patreon-tiers-members": {
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
