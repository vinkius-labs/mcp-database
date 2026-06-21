# Correios do Brazil MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/correios-do-brazil)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Calculate shipping costs, estimate delivery times, and consult address information via the official Correios REST API.

## Description
Connect your **Correios** account to any AI agent to automate logistics and shipping calculations directly within your workflow.

### What you can do

- **Shipping Calculation** — Calculate precise shipping costs based on origin, destination, weight, and package dimensions for services like SEDEX and PAC.
- **Delivery Estimates** — Get the estimated number of working days for any delivery across Brazil.
- **Address Lookup (CEP)** — Instantly retrieve full address details (street, neighborhood, city, state) from any Brazilian ZIP code.
- **Service Comparison** — Compare different postal service codes to find the best shipping option for your needs.

### How it works

1. Subscribe to this server
2. Enter your Correios Web Services (CWS) credentials
3. Start querying logistics data from Claude, Cursor, or any MCP client

### Who is this for?

- **E-commerce Owners** — quickly estimate shipping costs for customers without leaving the chat.
- **Developers** — verify address data and integrate logistics logic into applications via natural language.
- **Logistics Managers** — track delivery windows and optimize shipping routes across Brazil.


## Available Tools (3)
- **calculate_prices**: Calculate shipping cost for postal services
- **consult_cep**: Consult address information for a ZIP code
- **estimate_delivery_time**: Estimate delivery time between two ZIP codes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Correios do Brazil** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the shipping cost for a 1kg box (20x20x20cm) from 01001000 to 20040002 using SEDEX (04014)."

**🤖 AI Agent:**
> I've calculated the shipping for your SEDEX package. The estimated cost is R$ 32.50 with a delivery window of 1-2 business days.

---

**👤 You:**
> "How long does it take for a PAC delivery from 01310-200 to 70040-900?"

**🤖 AI Agent:**
> The estimated delivery time for PAC (service 04510) between these locations is 8 working days.

---

**👤 You:**
> "What is the address for CEP 01001000?"

**🤖 AI Agent:**
> The CEP 01001-000 corresponds to Praça da Sé, Sé, São Paulo - SP.


## ❓ FAQ

**Q: How can I calculate the shipping price for a specific package?**
Use the `calculate_prices` tool. You will need to provide the origin and destination ZIP codes, weight, dimensions, and the service code (e.g., 04014 for SEDEX).

**Q: Can I check the delivery deadline between two Brazilian cities?**
Yes! The `estimate_delivery_time` tool allows you to input the service code and both ZIP codes to receive the estimated delivery time in working days.

**Q: Is it possible to find an address using only the ZIP code (CEP)?**
Absolutely. Use the `consult_cep` tool with the 8-digit ZIP code to retrieve the street name, neighborhood, city, and state automatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/correios-do-brazil](https://vinkius.com/mcp/correios-do-brazil)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Correios do Brazil** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `correios-do-brazil` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Correios do Brazil** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "correios-do-brazil": {
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
