# FedEx MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fedex)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

AI logistics: track shipments, get rates, create shipments, and find locations via agents.

## Description
### What you can do

Connect AI agents to the FedEx API suite for end-to-end logistics management:

- **Track packages** in real-time with detailed scan history and delivery estimates
- **Track multiple packages** simultaneously for batch monitoring
- **Get shipping rates** across all FedEx services (Express, Ground, Freight)
- **Create shipments** and generate shipping labels directly
- **Validate addresses** to prevent delivery failures
- **Find nearby FedEx locations** (offices, drop boxes, ship centers)
- **Verify postal codes** and check service availability between locations
- **Get proof of delivery** documents for completed shipments

### How it works

1. **Get your FedEx API credentials** from the FedEx Developer Portal
2. **Ask your AI agent** to track shipments, quote rates, or create shipments
3. **Natural language commands** replace manual FedEx website navigation
4. **Production-ready data** directly from FedEx's operational systems

### Who is this for?

Essential for **e-commerce businesses**, **warehouse managers**, **shipping coordinators**, **customer support teams**, and **logistics professionals**. Let AI agents automate tracking updates, compare shipping costs, validate customer addresses, and find drop-off locations. Perfect for businesses shipping 10+ packages daily who want to eliminate manual tracking, streamline label generation, and reduce delivery exceptions through automated address validation.


## Available Tools (9)
- **create_shipment**: Requires shipper/recipient details, package weight/dimensions, and service type. Returns tracking number, label format, and estimated delivery date. Use this to generate labels for outbound shipments or process returns.

Create a FedEx shipment and generate a shipping label
- **get_postal_code**: Use this to verify postal codes before shipping or to resolve ambiguous addresses.

Validate a postal/ZIP code and get location details
- **check_service_availability**: Includes service names, transit times, and availability status. Use this to verify if Express, Ground, or Freight services operate between specific postal codes before quoting or booking shipments.

Check if FedEx shipping services are available between two locations
- **find_locations**: Includes location type (FedEx Office, Ship Center, Drop Box), address, hours of operation, and services offered. Use this to find where to drop off packages, print labels, or access packing supplies.

Find nearby FedEx locations (drop-off points, offices, or drop boxes)
- **get_proof_of_delivery**: Returns POD image URL, delivery date, recipient name, and signature status. Use this to confirm successful delivery for billing disputes, insurance claims, or customer inquiries.

Get proof of delivery (POD) document for a delivered FedEx package
- **get_rates**: Requires origin/destination postal codes, package weight, and dimensions. Returns service type, rate, currency, and estimated delivery date. Use this to compare shipping costs or choose the most economical service.

Get shipping rates and transit times for FedEx services
- **track_multiple_packages**: Returns an array of results with status, scans, and delivery info for each. Requires an array of tracking numbers. Use this for batch monitoring of multiple shipments or checking the status of a multi-piece delivery.

Track multiple FedEx packages in a single request
- **track_package**: Requires the 12-15 digit tracking number. Use this to monitor shipment progress, verify delivery, or investigate delays.

Track a single FedEx package by tracking number
- **validate_address**: Returns standardized format, validation status, and suggestions if the address is incorrect. Requires street lines, city, state, and postal code. Use this to prevent delivery failures, correct typos in addresses, or verify international addresses before shipping.

Validate and standardize a shipping address with FedEx


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FedEx** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Track package 123456789012 and tell me when it will be delivered"

**🤖 AI Agent:**
> I'll retrieve the tracking history and estimated delivery date for your package.

---

**👤 You:**
> "How much to ship a 5lb box from 10001 to 90210 via FedEx Ground?"

**🤖 AI Agent:**
> I'll get rate quotes for all available FedEx services between those ZIP codes.

---

**👤 You:**
> "Find the nearest FedEx drop-off location to 37201"

**🤖 AI Agent:**
> I'll search for FedEx locations near that ZIP code and show you the closest options.


## ❓ FAQ

**Q: Do I need a FedEx account to use this MCP server?**
For tracking and address validation, you only need free API credentials from the FedEx Developer Portal. For creating shipments and generating labels, a valid FedEx shipping account number is required.

**Q: Can this MCP server generate shipping labels?**
Yes! The create_shipment tool generates a shipping label (PDF format) and returns the tracking number. You'll need your FedEx account number, shipper/recipient details, and package specifications. The label is returned as a URL or encoded string ready for printing.

**Q: How many packages can I track at once?**
The track_multiple_packages tool allows tracking up to 30 packages in a single request. For larger batch tracking, you can make multiple requests. Each individual tracking request returns full scan history and delivery status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fedex](https://vinkius.com/mcp/fedex)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FedEx** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fedex` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FedEx** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fedex": {
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
