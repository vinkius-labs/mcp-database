# ShipCompliant MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shipcompliant)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/shipcompliant-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/shipcompliant-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Check wine shipping compliance, calculate alcohol taxes, verify licenses, and get state regulations for your Sovos ShipCompliant account through natural conversation.

## Description
Connect your **ShipCompliant by Sovos** account to any AI agent and navigate the complex world of US alcohol shipping compliance through natural conversation.

### What you can do

- **Compliance Check** — Verify if shipping wine/spirits from one state to another is legally compliant
- **Tax Calculation** — Calculate state-specific excise tax, sales tax, and alcohol surcharges for accurate invoicing
- **Shipping Rules** — Get detailed carrier restrictions, volume limits, temperature requirements, and signature rules by state
- **License Management** — View all your active, pending, and expired shipping licenses across all 50 states
- **State Regulations** — Deep-dive into any state's alcohol laws: age verification, volume caps, and product restrictions
- **Product Registry** — List all registered products with brand names, alcohol content, and approved states
- **Carrier Info** — View approved carriers for alcohol shipment with compliance certifications

### Who is this for?

- **DTC Shipping Managers** — Instant compliance checks before fulfilling orders
- **Winery Compliance Officers** — License tracking, renewal alerts, and regulatory updates
- **Wine Club Directors** — State eligibility for club shipments and volume cap monitoring
- **eCommerce Teams** — Tax accuracy for online wine sales across all 50 states


## Available Tools
- **check_compliance**: Returns compliance status, volume limits, license requirements, and any restrictions. THE most important tool — always check before shipping alcohol.

Check shipping compliance
- **calculate_tax**: Returns total tax amount and breakdown by tax type. Required for accurate invoicing.

Calculate alcohol tax
- **get_shipping_rules**: Get state shipping rules
- **list_licenses**: Critical for knowing where you can legally ship.

List your shipping licenses
- **check_license_status**: Returns license details and expiration date.

Check license status for a state
- **list_products**: List registered products
- **get_state_rules**: Get state alcohol rules
- **list_carriers**: List approved carriers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ShipCompliant** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can we ship Pinot Noir from California to Texas?"

**🤖 AI Agent:**
> 📋 **Compliance Check: CA → TX**

✅ **Shipping is COMPLIANT**

📜 **Your license**: TX DTC Permit #TX-2024-8847 — Active (expires Dec 2026)

📦 **Volume limits**:
- Per shipment: 9 liters max
- Annual per customer: 108 liters (12 cases)

💰 **Tax breakdown** (example: $45 bottle):
- TX excise tax: $0.204/gallon
- TX sales tax: 6.25% → $2.81
- Local tax: ~2% → $0.90
- **Total tax: ~$3.91/bottle**

📋 **Requirements**:
- ✅ Adult signature required (21+)
- ✅ Common carrier only (FedEx, UPS)
- ❌ USPS not permitted
- ✅ Shipped from licensed premises

---

**👤 You:**
> "Calculate alcohol taxes for a $50 bottle of wine shipped to New York."

**🤖 AI Agent:**
> 💰 **Tax Breakdown — CA → NY ($50 Bottle)**

- NY Excise Tax: $0.30/gallon
- State Sales Tax: 4.0% ($2.00)
- Local Tax (NYC): 4.875% ($2.44)
**Total Tax**: ~$4.44 per bottle

---

**👤 You:**
> "Show my active shipping licenses for California."

**🤖 AI Agent:**
> 📋 **Active Licenses: California**

1. **CA DTC Winegrower Permit**: #CA-9921-W
   - Expires: Dec 31, 2026
   - Status: Active

2. **CA Wholesale License**: #CA-WW-229
   - Expires: Jun 30, 2027
   - Status: Active

*(No pending renewals required)*


## Installation & Usage

To install and use the **ShipCompliant** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shipcompliant](https://vinkius.com/mcp/shipcompliant)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
