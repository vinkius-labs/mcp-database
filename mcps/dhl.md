# DHL MCP Server

AI logistics: track global shipments, audit delayed packages, and quote DHL worldwide rates.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dhl)

## Overview
**Category:** industry-titans
**Tools Count:** 6

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


## Available Tools
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


## Installation & Usage

To install and use the **DHL** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dhl](https://vinkius.com/mcp/dhl)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
