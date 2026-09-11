# Claro Antifraud (Open Gateway) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/claro-antifraud-open-gateway)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Line & location security checks on the official Claro Brasil gateway: SIM swap check and last-swap date (GSMA), line-change alerts (Claro Alerta), number recycling, device location verify/retrieval and legacy LBS — OAuth client_credentials.

## Description
**Line security and device location checks** on the official Claro Brasil API gateway (Claro Insight / GSMA Open Gateway) — everything an antifraud or risk agent needs to trust (or block) a mobile line.

### What you can do
- **SIM swap check** — has the SIM been swapped within the last N hours (up to 2400)? The classic account-takeover signal before password resets and high-value transactions
- **SIM swap date** — the exact timestamp of the last SIM change, for forensics and case review
- **Claro Alerta** — line-change alerts: SIM-chip swap, device change, MSISDN change, subscription cancel
- **Number recycling** — was the number assigned to a new owner since a given date? Validates stale customer databases
- **Device Location Verify** — is the device inside a lat/long circle (2-200 km)? returns verificationResult true/false (LGPD consent required)
- **Device Location Retrieval** — the device's last known location: circular area + timestamp
- **LBS Device Location** — cell-level last position from the legacy LBS platform (coordinates, accuracy radius, validation time)

### Authentication
1. Register an app in the **Claro Insight marketplace** (www.claro.com.br) to get a Client ID + Client Secret and your Customer ID (trials with 1.000 requests per API)
2. The MCP mints a token at `POST https://api.claro.com.br/oauth2/v1/token` (`grant_type=client_credentials`) and refreshes it automatically
3. Every call carries your marketplace Customer ID as the `X-CustomerID` header

### Who is this for?
Antifraud and risk agents, fintech onboarding flows, account-takeover detection, database hygiene and delivery/asset validation — anyone securing actions behind the trustworthiness of a phone line.


## Available Tools (7)
- **get_lbs_device_location**: Coarsest and cheapest of the location checks — use for asset/fleet monitoring and region-level checks. location_type "LAST" gives the most recent reading. The LBS service enforces a per-MSISDN rate ceiling: a 429 means you polled that number too often — back off rather than retry immediately. network_msisdn = country code + number, digits only ("5521912345678"). User consent applies under LGPD.

Get the last known cell-level location of a Claro device via the legacy LBS platform — coordinates, area type and accuracy radius
- **retrieve_device_location**: Use when you need where the device was (nearest-city level trust, asset tracking checks) rather than a yes/no inside-test. max_age_seconds limits how fresh the reading must be (e.g. "600" = only data up to 10 minutes old; omit for the freshest available). The device must be on the Claro mobile data network, and user consent is mandatory under LGPD — tell the user consent is required. phone_number in E.164, leading + optional.

Get the last known location of a device on the Claro network (GSMA Device Location retrieval) — area and timestamp
- **get_sim_swap_date**: Use when you need the exact moment rather than a yes/no — forensics, fraud case review, or deciding how stale a SIM-based authentication is. phone_number in E.164, leading + optional ("+5511999999999" or "5511999999999"). A response with no change date means no swap was recorded for the line.

Get the timestamp of the last SIM card change on a Claro phone number (GSMA SIM Swap retrieve-date)
- **get_line_change_alerts**: The strongest antifraud pattern: a SIM change right before a password reset or high-value transaction is classic account takeover. event_types defaults to "SIMCARD_CHANGED,DEVICE_CHANGED"; add MSISDN_CHANGED and SUBSCRIPTION_CANCELED when reviewing onboarding or fraud cases. Requires the optional credential CLARO_CUSTOMER_ID. network_msisdn = country code + number, digits only ("5521987654321").

Check recent operational changes on a Claro mobile line: SIM-chip swap, device change, number change, subscription cancel — the core account-takeover antifraud signal
- **check_number_recycling**: Use to validate stale databases: a number that was recycled means your stored customer data no longer belongs to that line, so registrations, contacts and marketing lists built on it are pointing at a stranger. specified_date = ISO 8601 date-time (e.g. "2025-01-01T00:00:00Z"); phone_number in E.164, leading + optional. Combine with get_sim_tenure for a full picture of the line's ownership stability.

Check whether a phone number was recycled (assigned to a new owner) since a given date (GSMA Number Recycling)
- **verify_device_location**: Use for fraud checks (falsified GPS), delivery validation and geofence spot-checks. accuracy_km between 2 and 200 (bigger = more forgiving). The check only works while the phone is connected to the Claro mobile data network, and user consent is mandatory under LGPD — tell the user consent is required before running it. phone_number may be sent with or without the leading "+" ("+5511974129777" or "+5511974129777"). To get the actual coordinates instead of a yes/no, use retrieve_device_location.

Verify whether a device is physically inside a given area (lat/long circle, 2-200 km radius) — returns verificationResult true/false
- **check_sim_swap**: Use before password resets, high-value transactions and session elevation: a recent SIM swap is the classic account-takeover signal. max_age_hours = how far back to look, 1 to 2400 hours, default 240 (10 days); shorter windows are stricter. phone_number in E.164, leading + optional ("+5511999999999" or "5511999999999"). To get the exact timestamp of the last swap instead, use get_sim_swap_date.

Check whether a Claro phone number had its SIM card swapped recently — the core account-takeover antifraud check (GSMA SIM Swap)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Claro Antifraud (Open Gateway)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Has the SIM of +5511999999999 been swapped in the last 24 hours?"

**🤖 AI Agent:**
> 🚨 **SIM Swap check: +5511999999999**

Queried with a 24-hour window: the response carries `swapped` — true means the chip changed hands right in the danger zone for account takeover.

Before allowing the password reset, also pull the exact swap timestamp with get_sim_swap_date for the case record. Want me to?

---

**👤 You:**
> "Was the number 5521912345678 recycled since January 2025?"

**🤖 AI Agent:**
> ♻️ **Number Recycling: 5521912345678**

Checked ownership since 2025-01-01: the response carries `recycled`. If true, any customer data you hold for that number now belongs to a stranger — registrations, contacts and marketing lists pointing at it need re-validation.

I can run get_sim_tenure on the same line to see how long the (possibly new) owner has been active. Want that?

---

**👤 You:**
> "Is the device of 5511974129777 within 5 km of -23.627, -46.655?"

**🤖 AI Agent:**
> 📍 **Device Location: 5511974129777**

Circle centred on -23.627, -46.655 with a 5 km radius: the response carries `verificationResult` true/false. Remember this check needs the phone on the Claro mobile data network and the user's LGPD consent.

Need the actual coordinates instead of a yes/no? I can pull the last known area with retrieve_device_location.


## ❓ FAQ

**Q: How do I get the credentials?**
Register at www.claro.com.br (Marketplace API Claro) and subscribe to the APIs you need — most offer a free trial with 1.000 requests for 3 months. The marketplace issues a Client ID, Client Secret and your Customer ID. This MCP exchanges them at POST https://api.claro.com.br/oauth2/v1/token (grant_type=client_credentials) for a bearer token (24h TTL) that it refreshes automatically; the Customer ID rides along as the X-CustomerID header on every call.

**Q: Which check should I use for account-takeover detection?**
check_sim_swap is the standard CAMARA signal (yes/no within an hour window, up to 2400h). For forensics use get_sim_swap_date for the exact timestamp, and get_line_change_alerts for Claro's own event stream (chip, device, MSISDN and subscription events). Device location checks are LGPD-sensitive: user consent is mandatory and the phone must be on the Claro mobile data network.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/claro-antifraud-open-gateway](https://vinkius.com/ai-agent-connect/claro-antifraud-open-gateway)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Claro Antifraud (Open Gateway)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `claro-antifraud-open-gateway` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Claro Antifraud (Open Gateway)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "claro-antifraud-open-gateway": {
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
