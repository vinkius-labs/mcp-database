# Lob MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lob-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Send physical mail programmatically with an API for postcards, letters, and checks that integrates into your digital workflows.

## Description
Connect your **Lob** account to any AI agent and manage direct mail through natural conversation.

### What you can do

- **Letter Sending** — Create and send letters with PDF or HTML content
- **Postcard Campaigns** — Send postcards with front/back designs
- **Check Printing** — Create and mail checks with payment details
- **Address Verification** — Verify and standardize US addresses
- **Template Management** — Browse and manage mail templates
- **Delivery Tracking** — Track mail pieces through the postal system

### How it works

1. Subscribe to this server
2. Enter your Lob API Key (test or live)
3. Start sending mail from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing** — run direct mail campaigns with postcards and letters
- **Finance** — automate check printing and mailing
- **Operations** — verify addresses and track mail delivery


## Available Tools (9)
- **autocomplete_address**: Suggest address completions
- **create_check**: Send a physical check
- **create_letter**: Supports certified mail and custom inserts.

Send a physical letter
- **create_postcard**: Supports HTML or PDF for front and back.

Send a physical postcard
- **get_mail_tracking**: Track a mail piece
- **list_letters**: List sent letters
- **list_postcards**: List sent postcards
- **verify_intl_address**: Verify an international address
- **verify_us_address**: Verify a US address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lob** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a welcome letter to a new customer and verify their address first."

**🤖 AI Agent:**
> Address verified! ✅ '123 Main St, Apt 4B, New York, NY 10001'. Deliverable: Yes. Type: Residential. Coordinates: 40.7484, -73.9967. Letter sent! ID: ltr_4521. To: John Smith. Pages: 2. Mail class: First Class. Expected delivery: Apr 30 — May 2. Cost: $0.92.

---

**👤 You:**
> "Show all mail pieces sent this month with delivery status."

**🤖 AI Agent:**
> This month: 45 mail pieces. Letters: 28, Postcards: 12, Checks: 5. Delivered: 38 (84%). In Transit: 5. Processing: 2. Returned: 0. Avg delivery: 3.2 days. Total cost: $52.40. Campaign 'Spring Promo' postcards: 12 sent, 10 delivered.

---

**👤 You:**
> "Create a check for $5,000 and browse mail templates."

**🤖 AI Agent:**
> Check created! ID: chk_8901. Amount: $5,000.00. To: Acme Corp, 456 Business Ave, Chicago, IL 60601. Memo: 'Q2 services payment'. Mail class: First Class. Expected delivery: May 1-3. Templates: 5 available. 'Welcome Letter' (HTML), 'Invoice Notice' (HTML), 'Thank You Card' (postcard), 'Payment Notice' (letter), 'Renewal Reminder' (postcard).


## ❓ FAQ

**Q: Can I send letters and postcards through the AI agent?**
Yes. Create and send letters with PDF/HTML content and postcards with custom designs. Track delivery through the postal system.

**Q: Does Lob use Basic Auth?**
Yes. Lob uses **HTTP Basic Auth** with the API Key as username (no password) against `api.lob.com/v1`.

**Q: Can I verify US addresses?**
Yes. Verify and standardize US addresses with CASS certification. Returns deliverability status, corrected addresses, and coordinates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lob-alternative](https://vinkius.com/mcp/lob-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lob** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lob-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lob** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lob-alternative": {
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
