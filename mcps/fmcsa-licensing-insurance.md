# FMCSA Licensing & Insurance MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fmcsa-licensing-insurance)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Access real-time FMCSA data to verify motor carrier licensing, insurance, safety ratings, and authority status directly through AI.

## Description
Connect your AI agent to the **Federal Motor Carrier Safety Administration (FMCSA)** database to perform deep due diligence on trucking companies and motor carriers. This server enables instant retrieval of official government records for compliance, safety, and operational verification.

### What you can do

- **Carrier Identification** — Search for carriers by Legal/DBA name or retrieve specific profiles using U.S. DOT or Docket numbers.
- **Safety & Compliance** — Access Carrier BASIC (Safety) measures and Out-of-Service (OOS) data to evaluate risk.
- **Operating Authority** — Verify the current status of a carrier's operating authority and associated docket numbers.
- **Operational Details** — Inspect authorized cargo types and operation classifications to ensure the carrier matches your logistics needs.

### How it works

1. Subscribe to this server
2. Enter your FMCSA Web Key
3. Start auditing carriers directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics Managers** — Instantly verify if a new carrier is authorized and insured before booking a load.
- **Compliance Officers** — Automate the monitoring of safety ratings and out-of-service orders for your fleet partners.
- **Freight Brokers** — Streamline the vetting process by pulling government data directly into your workflow.


## Available Tools
- **get_carrier_authority**: Retrieve operating authority status
- **get_carrier_basics**: S. DOT number.

Retrieve Carrier BASIC (Safety) measures
- **get_carrier_by_docket**: Retrieve carrier details by Docket Number
- **get_carrier_by_dot**: S. DOT number.

Retrieve carrier details by U.S. DOT number
- **get_carrier_cargo**: Retrieve types of cargo carried
- **get_carrier_dockets**: Retrieve associated docket numbers
- **get_carrier_oos**: Retrieve Out-of-Service (OOS) data
- **get_carrier_operation_class**: Retrieve operation classifications
- **search_carriers_by_name**: Supports pagination.

Search carriers by Legal or DBA name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FMCSA Licensing & Insurance** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for carriers with the name 'Blue Sky Logistics'."

**🤖 AI Agent:**
> I found 3 carriers matching 'Blue Sky Logistics'. The primary one is based in Ohio with DOT number 2938475. Would you like to see its full safety profile?

---

**👤 You:**
> "Get the safety BASIC measures and OOS data for DOT 1234567."

**🤖 AI Agent:**
> Retrieving safety data for DOT 1234567... The carrier has a 'Satisfactory' rating. Their Unsafe Driving BASIC is at 15% and they have 0 active Out-of-Service orders.

---

**👤 You:**
> "What types of cargo is carrier DOT 987654 authorized to carry?"

**🤖 AI Agent:**
> Checking cargo authorization for DOT 987654... This carrier is authorized for General Freight, Household Goods, and Refrigerated Food.


## ❓ FAQ

**Q: How can I check if a carrier is currently authorized to transport goods?**
You can use the `get_carrier_authority` tool with the carrier's DOT number. This will return the official operating authority status directly from FMCSA records.

**Q: Can I find a carrier's DOT number if I only have their business name?**
Yes, use the `search_carriers_by_name` tool. Provide the Legal or DBA name, and the agent will return a list of matching carriers along with their U.S. DOT numbers.

**Q: Does this tool show safety ratings and inspection violations?**
Yes. The `get_carrier_basics` tool retrieves safety performance data (BASIC measures), and `get_carrier_oos` provides data on Out-of-Service orders.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fmcsa-licensing-insurance](https://vinkius.com/mcp/fmcsa-licensing-insurance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FMCSA Licensing & Insurance** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `fmcsa-licensing-insurance` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FMCSA Licensing & Insurance** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fmcsa-licensing-insurance": {
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
