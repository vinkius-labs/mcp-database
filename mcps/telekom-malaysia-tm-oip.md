# Telekom Malaysia (TM) OIP MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/telekom-malaysia-tm-oip)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/telekom-malaysia-tm-oip-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/telekom-malaysia-tm-oip-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Orchestrate Telekom Malaysia (TM) services — manage broadband plans, service orders, and network usage directly from any AI agent.

## Description
Connect your AI agents to the **Telekom Malaysia (TM) Open Innovation Platform (OIP)**, the industry-standard ecosystem based on TM Forum Open APIs. This MCP provides 10 tools to manage the full lifecycle of telecommunication services, from querying broadband product catalogs and checking coverage availability to automating service orders and monitoring real-time data consumption.

### What you can do

- **Product Orchestration** — List available broadband and mobile offerings with technical specs and pricing
- **Service Fulfillment** — Create and track service orders (TMF 641) for new installations and upgrades programmatically
- **Usage Monitoring** — Retrieve granular data consumption reports and monitor network usage patterns for active services
- **Support & Billing** — List active trouble tickets and retrieve account billing details via natural language
- **Coverage Intelligence** — Verify service reachability for any Malaysian street address before placing orders

### How it works

1. Subscribe to this server
2. Register at the [**TM OIP Developer Portal**](https://store.oip.tm.com.my/)
3. Create an application in the API Manager to generate your **Consumer Key** and **Consumer Secret**
4. Subscribe to the relevant TMF APIs (Product Catalog, Service Ordering, etc.)
5. Insert your credentials into the fields below to start managing your telecommunication workflows.

### Who is this for?

- **System Integrators** — bridge enterprise portals with TM's official service provisioning backend
- **Property Managers** — automate broadband availability checks and installation requests for multiple sites
- **Network Ops** — monitor real-time usage and incident reports for multiple organizational accounts smoothly


## Available Tools
- **check_service_availability**: Verify broadband availability for a specific address
- **create_service_order**: Place a new service order for broadband or mobile
- **get_account_billing**: Get billing and account details for a customer
- **get_offering_details**: Get detailed information for a specific product offering
- **get_service_status**: Retrieve real-time status for a specific service
- **get_order_details**: Check the status of a specific service order
- **get_usage_report**: Monitor data consumption for a service
- **list_product_offerings**: List all broadband and telecom product offerings
- **list_active_services**: List active services in the inventory
- **list_trouble_tickets**: List active support and network trouble tickets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Telekom Malaysia (TM) OIP** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check broadband availability for address '123 Jalan Ampang, Kuala Lumpur'."

**🤖 AI Agent:**
> Connecting to TM OIP service qualification engine... Good news! Broadband services are available at that location. Supported services include UniFi Home 100Mbps and 300Mbps. Would you like to see the pricing for these plans?

---

**👤 You:**
> "List the top 3 unifi plans from the product catalog."

**🤖 AI Agent:**
> Retrieving TM product catalog... I've found the top 3 unifi offerings: 1. UniFi Home 800Mbps (ID: off_1), 2. UniFi Home 300Mbps (ID: off_2), 3. UniFi Home 100Mbps (ID: off_3). All plans include free installation. Would you like the full technical specs?

---

**👤 You:**
> "What is the data usage for service ID 'srv_tm_123' for the last month?"

**🤖 AI Agent:**
> Querying TM usage management... For service 'srv_tm_123', the total data consumed in the last 30 days was 450GB. Usage was highest during week 2 (150GB). Would you like a daily breakdown?


## Installation & Usage

To install and use the **Telekom Malaysia (TM) OIP** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/telekom-malaysia-tm-oip](https://vinkius.com/mcp/telekom-malaysia-tm-oip)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
