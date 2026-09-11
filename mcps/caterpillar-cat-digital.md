# Caterpillar Cat Digital MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/caterpillar-cat-digital)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Caterpillar Cat Digital APIs as an MCP: equipment diagnostic services, telemetry billing records and the public Cat AI Assistant configuration — api.cat.com gateway with Bearer auth from the Cat Developer Program.

## Description
**Caterpillar's Cat Digital equipment APIs** (api.cat.com gateway) as a single MCP server — operational data from connected CAT machines.

### What you can do
- **Equipment diagnostics** — diagnostic events and fault codes from connected Cat machines via the Cat Diagnostic Services product
- **Telemetry billing** — data-usage records tied to your app's telemetry subscription (monitor API consumption against plan limits)
- **AI Assistant config** — the public configuration endpoint of the Cat Digital AI assistant (guest access)

### Authentication (from the Cat Digital Developer Program)
1. Apply through the **Cat Digital Developer Program** — after approval you receive Bearer access tokens for your subscribed products
2. Paste the token into this MCP's credentials; it is sent as `Authorization: Bearer` on every call
3. Apigee error codes identify issues clearly: `401.006` = missing/invalid token, `400.006` = missing required fields, `404.001` = wrong path

### Who is this for?
Fleet managers, equipment health analytics, dealers, construction tech builders and AI agents that need authoritative Caterpillar machine data.


## Available Tools (3)
- **get_telemetry_billing**: Requires an approved Cat Digital app with the Telemetry product; useful to monitor API usage against plan limits.

Get telemetry billing records for your Cat equipment data usage
- **get_diagnostics_services**: Bearer auth via the credentials tab; 401.006 means the token is missing/invalid, 403 means the app lacks the product subscription.

Get Cat Diagnostic Services data (equipment diagnostic events and codes)
- **get_ai_assistant_config**: 400.006 lists missing required fields if any are mandated at request time.

Get the public Cat Digital AI Assistant configuration (guest access)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Caterpillar Cat Digital** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me diagnostic events from my Cat machines"

**🤖 AI Agent:**
> 🚜 **Cat Diagnostic Services**

Recent diagnostic events from your connected fleet:
- D6T Dozer (S/N ABC123): Fault code 4592-14, aftertreatment
- 320 Excavator (S/N DEF456): Sensor reading event, hydraulic temp

Each event includes machine S/N, code and timestamp. Want the billing side to check your telemetry usage too?

---

**👤 You:**
> "How much telemetry data usage have we billed this month?"

**🤖 AI Agent:**
> 📊 **Telemetry billing (Cat Digital)**

Current cycle: X GB across N machines, within your plan allowance. Per-machine breakdown included in the payload.

Useful to catch runaway data plans on job sites with poor connectivity. Want historical months for trend analysis?


## ❓ FAQ

**Q: How do I get the access token?**
Apply to the Cat Digital Developer Program (through Caterpillar's digital team / your dealer). After app approval you receive Bearer tokens scoped to your subscribed products (Diagnostics, Telemetry). The token is sent as Authorization: Bearer on every call.

**Q: I get 401.006 — what does it mean?**
Apigee code 401.006 = 'Missing Authorization header or token value' — the Bearer token was not sent or is invalid/expired. 400.006 = missing required fields in the request; 404.001 = wrong path.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/caterpillar-cat-digital](https://vinkius.com/en/ai-agent-connect/caterpillar-cat-digital)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Caterpillar Cat Digital** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `caterpillar-cat-digital` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Caterpillar Cat Digital** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "caterpillar-cat-digital": {
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
