# 99Minutos Express MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/99minutos-express)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/99minutos-express-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/99minutos-express-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Call physical couriers via AI using 99Minutos. Extract immediate Last-mile shipping quotes and trace vehicle checkpoints dynamically.

## Description
Connect your physical **Last-Mile Logistic Console (99Minutos)** to the Vurb architecture transforming Claude into a literal heavy dispatcher terminal for Same-Day delivery runs globally across LatAm.

### What you can do

- **Live Rate Estimations** — Feed two Zipcodes and retrieve instantly exactly how much it costs to call an Express or Next-Day fleet to move the goods natively.
- **Order Dispacthing** — Write 'Call a courier delivering at XYZ' and witness the integration creating real pickup missions requesting a vehicle seamlessly.
- **Route Auditing** — Scan active GPS hooks using `get_tracking` knowing where your package is residing effectively.
- **Zone Coverage Probe** — Ensure you're mapping correctly across massive territories searching if specific bounds sit within 99Minutos active grid ranges.

### How it works

1. Install node mapping.
2. Fetch your 99 API Bearer Code extracting from the merchant layout natively.
3. Turn simple phrases into logistic trucks moving merchandise regionally.

### Who is this for?

- **D2C Store Operators** — Trying to map heavy localized delivery runs avoiding third party apps.
- **Express App Engineers** — Scanning fast local point to point ranges directly executing backend codes.
- **Merchant Services Analytics** — Consolidating active run metrics looking at Delivery failure rates.


## Available Tools
- **cancel_order**: Void an active courier run
- **create_order**: Request a courier express delivery
- **create_store**: Register a new dispatch warehouse
- **create_webhook**: Inject an HTTP delivery ping receptor
- **get_order**: Get express delivery details
- **get_rates**: Check point-to-point same-day costs
- **get_tracking**: Pull real-time vehicle geographical statuses
- **list_coverage**: Check LatAm ZIP code active coverage
- **list_orders**: List active express orders
- **list_return_orders**: Watch reverse logistics flows
- **list_stores**: List registered physical stores/nodes
- **list_webhooks**: Scan infrastructure active webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **99Minutos Express** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find out exactly how much it costs right now a Same-Day deployment taking my package picking up from 14002 ending at 16003."

**🤖 AI Agent:**
> Rates extracted actively from the logistics hub natively. Connecting point 14002 to 16003 yields an estimation of roughly $85 MXN applying under the classic 'sameday' ruleset capacity. Would you like me to ping the order and dispatch natively?

---

**👤 You:**
> "Query the grid tracking node extracting recent geographic updates pushing for order NN-7729."

**🤖 AI Agent:**
> Sourced heavily! Digging into tracking loops revealed NN-7729 shows state 'On Route'. Valid GPS logs register moving out of hub 30 minutes ago safely. Courier identity attached natively. ETA preserved clean.

---

**👤 You:**
> "List my physical stores"

**🤖 AI Agent:**
> Here.


## Installation & Usage

To install and use the **99Minutos Express** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/99minutos-express](https://vinkius.com/mcp/99minutos-express)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
