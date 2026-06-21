# DHL MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dhl)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

AI logistics: track global shipments, audit delayed packages, and quote DHL worldwide rates.

## Description
### What you can do

Connect AI agents to the **DHL Express Enterprise API** for global supply chain visibility:

- **Track shipments:** Audit real-time checkpoints, transit statuses, and projected delivery hours.
- **Get shipping rates:** Evaluate instant Express Worldwide and Economy quotes before issuing AWB.
- **Create shipments:** Dispatch logistics algorithms setting sender/recipient vectors automatically.
- **Validate compliance:** Certify delivery postal codes mapping to functional address routes cross-border.
- **Find service nodes:** Query precise GPS mapping of close DHL drop-off or pickup spots.

### How it works

1. Subscribe to this server
2. Enter your DHL App Credentials (Client ID, Secret, and Account Number)
3. Start managing your logistics operations natively via LLM


## Available Tools (6)
- **create_shipment**: Requires shipper/recipient details, package weight, and service type. Use this to generate labels for outbound shipments. Returns the tracking number and label document URL.

Create a DHL shipment and generate a shipping label
- **find_locations**: Includes address, opening hours, and services available. Use this to find where to drop off a package or visit a DHL center.

Find nearby DHL service locations
- **get_proforma_invoice**: Use this for customs clearance documentation or proof of value.

Retrieve the proforma invoice document for a DHL shipment
- **get_rates**: g., Express Worldwide, Economy Select) between origin and destination. Requires origin/recipient addresses and package details (weight, dimensions). Use this to compare shipping costs and delivery speeds.

Get shipping rates and transit times for DHL services
- **track_shipment**: Returns current status, delivery estimate, and detailed checkpoints (origin, destination, customs, etc.). Requires the 10-digit tracking number (e.g., 1234567890). Use this to monitor international or domestic deliveries.

Track a DHL shipment by tracking number
- **validate_address**: Returns standardized address format and suggestions if the address is incorrect. Use this to prevent delivery failures before creating a shipment.

Validate a DHL shipping address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DHL** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Investigate the real-time exact customs and logistics status for DHL waybill 1928374650."

**🤖 AI Agent:**
> I checked DHL's core network. Shipment 1928374650 is currently at 'Customs clearance status updated' in Cincinnati Hub, USA. It's scheduled for delivery tomorrow before end of day.

---

**👤 You:**
> "Evaluate the logistics rates for sending a 5-kilogram package from ZIP 10001 (US) to ZIP 80331 (DE)."

**🤖 AI Agent:**
> For a 5kg package from US (10001) to Germany (80331), DHL Express Worldwide costs approximately $145.20 USD with a 2-day transit time. Economy Select costs $89.50 with a 5-day transit.

---

**👤 You:**
> "Where is the closest official DHL drop-off service center near ZIP 90210?"

**🤖 AI Agent:**
> The nearest official DHL Service Point to 90210 is located on Santa Monica Blvd, 1.2 miles away. It accepts drop-offs until 6:00 PM local time today.


## ❓ FAQ

**Q: Does it track regular post or only DHL Express?**
This MCP is primarily optimized for the DHL Express system, checking 10-digit Air Waybill tracking numbers globally securely.

**Q: Can I automatically calculate cross-border freight costs?**
Yes. The AI can utilize the Rates Engine comparing weights and postal codes immediately providing exact prices.

**Q: How do I get API Credentials?**
Visit developer.dhl.com, create an account, register an App mapping to your DHL Express Account number, and inject the Client ID and Secret.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dhl](https://vinkius.com/mcp/dhl)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DHL** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dhl` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DHL** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dhl": {
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
