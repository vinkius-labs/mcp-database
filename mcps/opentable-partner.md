# OpenTable Partner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/opentable-partner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

OpenTable partner APIs as an MCP: real-time table availability, booking policies, reservation feeds, guest CRM sync, POS data and diner reviews — official platform API with OAuth2 client_credentials.

## Description
**OpenTable partner platform APIs** (platform.opentable.com) as a single MCP server — the same endpoints used by POS integrators and restaurant tech on the OpenTable network.

### What you can do
- **Real-time availability** — live reservation slots per restaurant (rid), party size and time window, with experiences and table-type filters
- **Booking policies** — rules that apply to a specific slot: cancellation windows, deposits, card requirements
- **Reservation feed** — all reservations in a scheduled-time window per restaurant (POS/partner scope)
- **Guest CRM sync** — incremental guest profile pulls with email opt-in filter (updated_after deltas)
- **POS data** — orders/spend linked to reservations for revenue analytics
- **Reviews** — review summary and individual diner reviews with reply references

### Authentication (from the official OpenTable Postman collection)
1. Become an **OpenTable partner** (restaurants and POS/tech integrators) — your app receives a Client ID + Client Secret
2. The MCP mints a Bearer token at `{oauth-url}/api/v2/oauth/token?grant_type=client_credentials` with HTTP Basic (client_id:client_secret) and caches it
3. All calls go to `https://platform.opentable.com/...` with `Accept: application/json`

### Who is this for?
Restaurant operators, POS/CRM integrators, hospitality analytics and AI agents building on live OpenTable booking data.


## Available Tools (6)
- **get_pos_data**: Requires POS integration on the restaurant.

Get POS data linked to reservations (orders, tickets, spend)
- **get_availability**: include_experiences=true adds special experiences; require_attributes filters table types. rid comes from your partner dashboard (e.g. 1038007).

Get real-time table availability for a restaurant (slots per party size)
- **get_booking_policies**: Get booking policies of a restaurant for a specific time slot (rules, cancellation, deposit)
- **list_reservations**: Pagination via limit/offset. Partner/POS integration scope.

List reservations for a restaurant in a scheduled-time window (live booking feed)
- **list_guests**: email_optin=true returns only opt-in guests. Use updated_after for deltas instead of full pulls.

List guest profiles synced from OpenTable (CRM sync, email opt-in filter)
- **get_restaurant_reviews**: Requires the Reviews product.

Get restaurant review summary and latest reviews from the OpenTable network


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenTable Partner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What tables are free tonight at 7pm for 4 people (rid 1038007)?"

**🤖 AI Agent:**
> 🍽️ **Availability rid 1038007 @ 19:00 (party 4)**

Slots found (±15 min):
- 18:45 — Standard table
- 19:00 — Standard table
- 19:30 — Patio (experience)

Booking policy at 19:00: card required, free cancellation until 24h before. Want policies for the 18:45 slot?

---

**👤 You:**
> "Sync all guests updated since Monday"

**🤖 AI Agent:**
> 👥 **Guest sync (rid 1038007, updated_after Monday)**

47 updated profiles (32 email opt-in):
- New reservations added for 9 guests
- 4 changed contact details
- 2 opted out of marketing

Deltas stored for your CRM. Want POS spend linked to their recent visits?

---

**👤 You:**
> "What are my latest OpenTable reviews saying?"

**🤖 AI Agent:**
> ⭐ **Latest diner reviews (rid 1038007)**

Average: 4.6/5 across 812 reviews

Latest 5: service praised twice, one 3-star mentioning slow desserts, two 5-stars on the tasting menu.

Want the full text of any review, or to check if any have unanswered replies?


## ❓ FAQ

**Q: How do I get OpenTable API credentials?**
Access is partner-gated: restaurants and POS/tech integrators join the OpenTable partner network (opentable.com/restaurant-solutions/api-partners). After approval, your app receives a Client ID + Client Secret; the OAuth client_credentials flow mints the Bearer token.

**Q: How does the guest CRM sync scale?**
Use updated_after with the timestamp of your last successful sync — the API returns only changed profiles (deltas), with limit/offset paging. This avoids full pulls and keeps your CRM in sync efficiently.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/opentable-partner](https://vinkius.com/en/ai-agent-connect/opentable-partner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenTable Partner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `opentable-partner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenTable Partner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "opentable-partner": {
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
