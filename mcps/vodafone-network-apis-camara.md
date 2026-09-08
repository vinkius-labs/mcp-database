# Vodafone Network APIs (CAMARA) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/vodafone-network-apis-camara)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Vodafone Developer Marketplace network APIs as an MCP: phone number verification, SIM swap detection (fraud), device status/location — CAMARA-compliant official APIs with OAuth2 client_credentials.

## Description
**Vodafone Developer Marketplace** network APIs — CAMARA-compliant (GSMA Open Gateway) official network capability APIs as a single MCP server.

### What you can do
- **Number verification** — passwordless check that a mobile number belongs to the device making the request (no SMS codes)
- **SIM swap detection** — was the SIM swapped recently? The strongest account-takeover signal in mobile banking; also retrieve the exact swap date
- **Device status & location** — is the device connected, roaming, on WiFi? Approximate location area for logistics and licensing

### Authentication (from the official docs)
1. Create a free developer account at **developer.vodafone.com** and create a sandbox app — you receive a Consumer Key + Consumer Secret and a per-product token endpoint
2. The MCP mints tokens at your app's **token endpoint** with HTTP Basic (consumer key:secret) + `grant_type=client_credentials&scope=`
3. Access tokens last **59 minutes 59 seconds with no refresh token** — the MCP re-mints automatically at 55 min
4. Every call carries the **vf-trace-transaction-id** header required by Vodafone for support tracing

### Available products (30 APIs in the marketplace)
Number Verification, SIM Swap, Age Verification (GB), Verified Caller, Brand Registration, Active Subscriber, Home Network Check, Call Divert, Number Recycling, MVNO Discovery, Onboarding & Ordering (TMF931) and more — sandbox is free; live access needs a production agreement per market (DE, GB, IE, NL, ES, GR, RO, PT, QA, ZA).

### Who is this for?
Fintech/fraud teams, fintech builders, telecom app developers, identity platforms and AI agents that need network-grade trust signals.


## Available Tools (6)
- **check_sim_swap**: 164) and optional maxAge (days, default 240) — returns {swapped: true|false}. SIM swap within a recent window is a strong account-takeover signal. Requires the SIM Swap product.

Check whether a SIM swap happened on a phone number recently (fraud prevention)
- **get_device_phone_number**: Useful to auto-fill forms and identify the user without manual input.

Get the phone number of the device making the request (CAMARA)
- **verify_number**: 164, e.g. "+447700900123") — returns {devicePhoneNumberVerified: true|false}. Ideal for passwordless login and fraud prevention. Requires the Number Verification product on your Vodafone app.

Number Verification: verify that a mobile number belongs to the device making the request (CAMARA)
- **get_device_status**: — returns connectivity status of the device: connected, deviceClass, roaming flag. Useful for smart delivery, automotive and IoT scenarios. Requires the Device Status product.

Get device connectivity status: is it reachable, roaming, on WiFi?
- **get_sim_swap_date**: 164) — returns {latestSimChange: ISO date} or null if no swap recorded. Compliance-grade evidence for fraud investigations. Requires the SIM Swap product.

Get the exact date of the last SIM swap for a phone number
- **get_device_location**: device = {"phoneNumber":"+447700900123"} or IP. Requires the Device Location product.

Get the location area of a device (CAMARA Location Verification/Retrieval)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vodafone Network APIs (CAMARA)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify that phone number +447700900123 belongs to this device"

**🤖 AI Agent:**
> 📶 **Number Verification (CAMARA)**

Result: ✅ **devicePhoneNumberVerified: true**

The SIM in the current network session matches the number — passwordless login can proceed without SMS codes. Ideal for fintech onboarding.

---

**👤 You:**
> "Was there a SIM swap on this number in the last 90 days?"

**🤖 AI Agent:**
> 🔒 **SIM Swap check**

Result: ✅ **swapped: false** (look-back window 240 days)

No SIM swap detected — the account-takeover risk signal is clear. I can also retrieve the exact date of the last swap if one had occurred.

---

**👤 You:**
> "Is this device connected and roaming?"

**🤖 AI Agent:**
> 📶 **Device status**

- Connected: ✅ true
- Roaming: ❌ false (home network)
- Device class: smartphone

Useful before triggering push notifications or high-bandwidth features. Want location area as well?


## ❓ FAQ

**Q: How do I get the credentials?**
Create a free account at developer.vodafone.com, pick an API from the catalogue, and create a sandbox app — you get a Consumer Key + Consumer Secret plus the per-product Token URL and API Base URL to paste into this MCP's credentials. Live access requires a production agreement per market.

**Q: Why do the token URL and API base URL differ per product?**
Vodafone scopes each product separately: the token endpoint includes the product scope, so each app+product pair has its own token URL and API base URL — both are shown on your app's credentials page in the marketplace. The MCP takes both as credentials.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/vodafone-network-apis-camara](https://vinkius.com/ai-agent-connect/vodafone-network-apis-camara)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vodafone Network APIs (CAMARA)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vodafone-network-apis-camara` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vodafone Network APIs (CAMARA)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vodafone-network-apis-camara": {
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
