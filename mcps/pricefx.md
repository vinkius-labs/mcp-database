# Pricefx MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pricefx)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Equip your AI with advanced enterprise CPQ capabilities — fetch products, manage customers, and generate automated pricing quotes directly via chat.

## Description
Harness the power of **Pricefx**, the premier Cloud Pricing Optimization platform, by coupling it directly to your LLM agents. Empower your AI to navigate vast B2B catalogs, securely read customer pricing grids, and orchestrate automated Quote generation (CPQ) instantaneously via natural language prompts.

### What you can do

- **Live Catalog & Pricing** — Search deep into the `fetch_products` logic to find base SKUs, and evaluate their explicit Price Math limits via `get_product`
- **CRM & Account Rules** — Query your partition tracing active CRM records via `fetch_customers`, or force new structures dynamically (`create_customer`)
- **Quote Engine (CPQ)** — Ask the AI to build dynamic Quotes on the fly (`create_quote`) calculating complex arrays, or trace why an exist Quote ID failed approval (`get_quote`)
- **Seamless Deletion** — Obliterate drafted quotes matching strict constraints from your Partition without accessing the Gateway (`delete_quote`)

### How it works

1. Subscribe to this MCP server
2. Provide your Pricefx Cluster, Partition Name, and active JWT Token
3. Engage Claude, Cursor, or any compatible client to navigate the Pricing Engine natively

Forget executing long, structured JSON payloads through Postman. Just tell your AI: 'Create a new Quote for Customer XYZ with Product 123'. The agent handles the structural formatting and API syntax inherently.

### Who is this for?

- **Pricing Managers** — instantly check live Price Grids or simulate logic without waiting for heavy partition dashboards to load
- **Backend Devs** — test dynamic JSON payloads for Quote generation interacting intuitively to build headless frontends
- **Sales Engineers** — quickly pull the math trace behind a specific Quote ID during high-pressure B2B negotiations


## Available Tools
- **create_customer**: Ensure JSON format is robust.

Provision a highly-available JSON Payload generating hard Customer bindings
- **create_quote**: Retrieve the exact structural matching verifying CPQ Generation
- **delete_quote**: Irreversibly vaporize explicit validations extracting rich Churn flags
- **fetch_customers**: Identify bounded CRM records inside the Headless Pricefx Platform
- **fetch_products**: Enumerate explicitly attached structured rules exporting active pricing Catalog
- **fetch_quotes**: Identify precise active arrays spanning native Gateway auth
- **get_customer**: Perform structural extraction of properties driving active Account logic
- **get_product**: Retrieve explicit Cloud logging tracing explicit Product limits
- **get_quote**: Dispatch an automated validation check routing explicit Quote history
- **update_customer**: Provide bulk bounds strictly formatted.

Inspect deep internal arrays mitigating specific Plan Math


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pricefx** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you fetch all our active Quotes and find any that are still in Draft status?"

**🤖 AI Agent:**
> Querying `fetch_quotes`. I found 35 recent quotes mapped in your partition. Exactly 4 of them are flagged as `DRAFT`. Quote IDs `Q-990` and `Q-991` belong to Customer 105, indicating stalled approvals in their pipeline.

---

**👤 You:**
> "We need to create a new customer record manually. Give me the JSON for a generic B2B profile named `Acme Corp`."

**🤖 AI Agent:**
> I've structured the payload and fired `create_customer`. The array injected `{"customerId": "ACM-001", "name": "Acme Corp", "status": "ACTIVE"}` mapping natively into the CPQ core. The partition confirms success, generating internal Pricefx node ID 8841.

---

**👤 You:**
> "Look up product ID 'MX-Mouse-001'. Tell me its base price bracket before discounts."

**🤖 AI Agent:**
> Using `get_product` to hit the Pricing Gateway natively. For `MX-Mouse-001`, the specific arrays return a base ceiling of `49.99 USD`. The explicit attribute tree dictates no hard floor restrictions for Tier-1 Accounts.


## ❓ FAQ

**Q: Can the AI automatically assemble the correct JSON format for creating quotes?**
Yes, perfectly. By calling `create_quote`, you simply tell the AI: "Make a quote for customer 105 for product XYZ". It understands Pricefx schemas and writes the robust JSON mapping necessary to fulfill the API logic.

**Q: Does the server handle Pricefx partitioned clusters natively?**
Yes. Pricefx securely isolates environments based on `Cluster` (e.g., `eu1`, `us1`) and `Partition` names. Our server intrinsically limits the AI to operate strictly within the bounds you configure.

**Q: If a quote creation fails due to business rules, will the AI tell me why?**
Absolutely. If the CPU logic returns a rejection—like a discount violating a minimum margin—the AI extracts the raw API traceback identifying the specific pricing constraint that halted generation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pricefx](https://vinkius.com/mcp/pricefx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pricefx** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pricefx` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pricefx** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pricefx": {
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
