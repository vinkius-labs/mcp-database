# Correios (Brazil) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/correios-brazil)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Orchestrate Correios logistics — track objects, calculate shipping prices, and validate Brazilian addresses directly from any AI agent.

## Description
Connect your AI agents to **Correios**, the official national postal service of Brazil. This MCP provides 9 tools to automate real-time object tracking, calculate shipping deadlines and prices (PAC, SEDEX), and retrieve accurate address information using Brazilian zip codes (CEP) directly through natural conversation.

### What you can do

- **Logistics Orchestration** — Track multiple packages and retrieve granular status updates and historical events
- **Shipping Intelligence** — Calculate delivery deadlines and prices for various services between any two zip codes
- **Address Validation** — Retrieve complete street, neighborhood, and city details for any Brazilian CEP
- **Business Integration** — Access organizational contract configurations and list authorized service codes programmatically
- **Regional Insights** — Verify the state and city information associated with specific postal zones

### How it works

1. Subscribe to this server
2. Log in to the [**Correios Web Services Portal**](https://cws.correios.com.br/)
3. Navigate to **API Management** to obtain your **Username**, **Password**, and **Contract Number** (if applicable)
4. Identify your **Card ID** for specific billing configurations
5. Insert your credentials into the fields below to start managing your Brazilian logistics.

### Who is this for?

- **E-commerce Developers** — automate shipping calculations and tracking updates for Brazilian customers
- **Operations Managers** — monitor large volumes of outbound shipments via natural language
- **Customer Support Teams** — quickly provide real-time package statuses and address validation


## Available Tools (8)
- **calculate_price_deadline**: Calculate shipping price and delivery deadline
- **get_contract_status**: Check the current status of your Correios contract
- **get_unit_info**: Get details for a specific post office unit
- **list_contract_services**: , associated with your account.

List all postage services available in your contract
- **list_unit_types**: List all types of Correios units
- **lookup_cep**: Get address information from a Brazilian ZIP code (CEP)
- **search_units_by_cep**: Search for nearby post office units
- **track_object**: Track a package status using its tracking code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Correios (Brazil)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Track Correios object 'QI123456789BR' and show its latest status."

**🤖 AI Agent:**
> Connecting to Correios tracking service... Object 'QI123456789BR' was 'Delivered' (Objeto entregue ao destinatário) today at 2:30 PM in São Paulo, SP. Would you like me to see the full movement history?

---

**👤 You:**
> "Calculate shipping for a 2kg box from CEP 01310-100 to 20040-002."

**🤖 AI Agent:**
> Querying Correios price and deadline engine... For a 2kg package from SP to RJ: 1. SEDEX (R$ 35.50, 1 business day), 2. PAC (R$ 22.10, 5 business days). Which service would you like to choose?

---

**👤 You:**
> "Find the address details for CEP '01310-914'."

**🤖 AI Agent:**
> Searching Brazilian zip codes... CEP 01310-914 corresponds to: Avenida Paulista, 1159, Bela Vista, São Paulo - SP. This is a business district zone.


## ❓ FAQ

**Q: Can my AI automatically track a package just by providing the tracking code?**
Yes! Use the `track_object` tool with the tracking code (e.g., 'QI123456789BR'). Your agent will retrieve the current status, location, and the full history of logistics events.

**Q: How do I calculate shipping prices for PAC or SEDEX?**
Use the `calculate_shipping` tool with the origin and destination CEPs, along with the weight and dimensions of the package. The agent will return the estimated price and delivery deadline.

**Q: Can I retrieve the full address details from a zip code (CEP)?**
Yes! The `search_cep` tool allows your agent to fetch the street name, neighborhood, city, and state associated with any valid Brazilian zip code.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/correios-brazil](https://vinkius.com/mcp/correios-brazil)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Correios (Brazil)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `correios-brazil` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Correios (Brazil)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "correios-brazil": {
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
