# TollGuru MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tollguru-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Global toll intelligence — calculate costs by address, coordinates, polyline, or GPS tracks with fuel estimates and multi-vehicle support.

## Description
Equip your AI agent with the most accurate toll intelligence available via **TollGuru**. This unified server provides your agent with instant access to toll costs, fuel consumption estimates, and route optimization for thousands of roads worldwide. Your agent can instantly calculate the total cost of a journey, audit individual toll booth prices, and suggest the most cost-effective path without you ever checking a map or calculator manually. Whether you are planning long-haul logistics or optimizing a personal road trip, your agent acts as a dedicated travel cost analyst through natural conversation.

### What you can do

- **Cost Calculation** — Calculate exact toll costs for any route between two or more addresses.
- **Vehicle Optimization** — Specify different vehicle types (Auto, Taxi, Truck) to get tailored pricing and technical details.
- **Route Auditing** — Fetch detailed summaries of individual toll charges and payment methods (Tag, Cash).
- **Logistics Intelligence** — Analyze total journey costs including fuel and tolls to optimize organizational planning.
- **Global Coverage** — Access toll data for thousands of bridges, tunnels, and highways across the globe.

### How it works

1. Subscribe to this server
2. Enter your TollGuru API Key
3. Start managing your travel intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics & Supply Chain Managers** — instantly retrieve exact shipping costs and optimize routes for fleet efficiency.
- **Travelers & Road Trippers** — plan their budgets accurately by knowing toll and fuel costs in advance.
- **Delivery & Ride-share Drivers** — audit daily expenses and find the most profitable routes through natural language.
- **SaaS Developers** — integrate complex toll and route pricing into their applications via an AI-guided interface.
- **Financial Controllers** — monitor corporate travel expenses and verify individual toll receipts.


## Available Tools
- **calculate_tolls_by_address**: Supports multiple vehicle types.

Calculate tolls and fuel costs between two addresses
- **calculate_tolls_by_coordinates**: Returns multiple route options with toll breakdowns.

Calculate tolls between two GPS coordinate pairs
- **calculate_tolls_by_gps**: Handles map-matching automatically for accurate toll identification from real trip data.

Calculate tolls from GPS track data (post-trip reconciliation)
- **calculate_tolls_by_polyline**: Submit the encoded polyline string to get toll costs for that exact path.

Calculate tolls for an encoded route polyline
- **get_toll_rates**: Look up toll rates for a specific toll plaza or booth
- **get_transaction_count**: Useful for monitoring usage and billing.

Get total API transaction count for your account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TollGuru** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate tolls from New York to Philadelphia for a standard car."

**🤖 AI Agent:**
> Retrieving route costs from NYC to Philly... For a 2-axle auto, the total toll cost is approximately $25.50 using a tag or $32.00 in cash. I can list the individual tolls like the Holland Tunnel and NJ Turnpike.

---

**👤 You:**
> "What is the cheapest route from San Francisco to Los Angeles considering tolls?"

**🤖 AI Agent:**
> Analyzing routes between SF and LA... I've found a path with zero tolls taking the I-5 S, though it may take slightly longer. The alternative route via the coastal highway has $15 in bridge tolls. Which one do you prefer?

---

**👤 You:**
> "How much does a 5-axle truck pay in tolls from Chicago to Miami?"

**🤖 AI Agent:**
> Fetching heavy vehicle rates for the Chicago-Miami corridor... For a 5-axle truck, the total estimated toll cost is $145.00. I have the breakdown of state-by-state charges and tag vs cash options ready for you.


## ❓ FAQ

**Q: Can I calculate tolls for multiple vehicle types like cars and trucks?**
Yes! All toll calculation tools (`calculate_tolls_by_address`, `calculate_tolls_by_coordinates`, `calculate_tolls_by_polyline`, `calculate_tolls_by_gps`) accept a `vehicle_type` parameter. Supported types include `2AxlesAuto`, `2AxlesTaxi`, `2AxlesMotorcycle`, `3AxlesTruck`, and up to 9-axle configurations.

**Q: Does the result show both cash and electronic tag prices?**
Absolutely. The `TollPresenter` displays the costs for different payment methods whenever available from the API, allowing you to choose the best option.

**Q: What addresses should I use for origin and destination?**
You can provide full physical addresses, city names, or even specific coordinates. The more precise the address, the more accurate the toll calculation will be.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tollguru-alternative](https://vinkius.com/mcp/tollguru-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TollGuru** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `tollguru-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TollGuru** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tollguru-alternative": {
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
