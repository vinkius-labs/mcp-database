# Zenoti MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zenoti)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage guests, appointments, therapists, invoices, memberships, and gift cards for your Zenoti-powered spa or salon enterprise through natural conversation.

## Description
Connect your **Zenoti** organization to any AI agent and manage your spa, salon, or medspa enterprise through natural conversation.

### What you can do

- **Guests** — Search guests, view profiles, preferences, allergies, and loyalty points
- **Appointments** — Browse bookings with therapist, room, service, and payment status
- **Services** — List all spa/salon services with pricing, duration, and categories
- **Therapists** — View providers with specialties, ratings, and availability
- **Invoices** — Track revenue, sales, tips, and payment breakdowns
- **Memberships** — Manage membership tiers: basic, premium, VIP, couples
- **Packages** — Browse bundled services: couples massage, day spa, bridal
- **Gift Cards** — Track gift card balances, sales, and redemptions
- **Centers** — Manage multi-location operations across your enterprise

### Who is this for?

- **Massage Envy, Hand & Stone, European Wax Center** — Built for franchise-scale spa operations
- **Spa Directors** — Real-time revenue, therapist utilization, and guest satisfaction data
- **Regional Managers** — Compare performance across all centers
- **Front Desk** — Instant guest lookup, appointment details, and loyalty info


## Available Tools
- **list_centers**: Includes name, address, timezone, and operating hours. Essential for multi-location spa chains like Massage Envy.

List spa/salon locations
- **list_employees**: Includes role, schedule, payroll info, and commission structure.

List all employees
- **list_invoices**: Filter by date range for revenue analysis.

List sales and invoices
- **list_memberships**: Shows pricing, included services, visit limits, and perks.

List membership plans
- **list_packages**: Shows included services and pricing.

List service packages
- **list_gift_cards**: Filter by guest to see a specific person's cards.

List gift cards
- **get_center**: Get center details
- **search_guests**: Returns profile, visit history, loyalty points, preferred therapist, and product preferences.

Search spa/salon guests
- **get_guest**: Get guest profile
- **get_guest_loyalty**: Get guest loyalty points
- **list_appointments**: Filter by date to see a specific day.

List spa/salon appointments
- **get_appointment**: Get appointment details
- **list_services**: Includes pricing, duration, category, and required room type.

List spa/salon services
- **list_therapists**: List therapists and providers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zenoti** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show today's appointments at the downtown center."

**🤖 AI Agent:**
> Downtown Spa — Today's appointments:

🧖 9:00 AM — **Jessica M.** 90-min Deep Tissue with Mark (Room 3) — $165
💆 10:00 AM — **Sarah K.** Anti-Aging Facial with Ana (Room 1) — $120
💅 10:30 AM — **Amanda R.** Gel Manicure + Pedicure with Lisa (Station 4) — $85
🧖 11:30 AM — **David L.** Hot Stone Massage with Maria (Room 2) — $145

4 appointments, $515 projected revenue. Room 3 is open from 12:00–3:00 PM.

---

**👤 You:**
> "Find the profile for guest Maria Gonzalez and check her loyalty points."

**🤖 AI Agent:**
> Accessing Zenoti guest records ('get_guest')...
Maria Gonzalez (Guest ID: G-44291):
- Membership: Gold VIP Tier
- Loyalty Points: 4,500 (Value: $45.00)
- Preferences: Prefers female therapists, deep tissue pressure.
- Last Visit: Sept 20th.

---

**👤 You:**
> "What is the total revenue collected across all centers today?"

**🤖 AI Agent:**
> Running real-time enterprise report ('get_revenue_report')...
Enterprise Daily Totals (As of 3:45 PM):
- **Total Revenue**: $24,850.00
  - Services: $16,200.00
  - Retail: $3,400.00
  - Memberships: $5,250.00
Top Center: Downtown ($6,400). Lowest: North Creek ($1,200).


## ❓ FAQ

**Q: Which brands use Zenoti?**
Zenoti powers 30,000+ locations worldwide including Massage Envy, Hand & Stone, European Wax Center, Massage Heights, Woodhouse Spas, and thousands of independent luxury spas and salons.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zenoti](https://vinkius.com/mcp/zenoti)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zenoti** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zenoti` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zenoti** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zenoti": {
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
