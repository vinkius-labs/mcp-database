# DOT Transportation / 美国交通部 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dot-transportation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Official U.S. DOT transportation data — decode VINs, check safety recalls, and audit ratings via AI.

## Description
Empower your AI agent to orchestrate your automotive research and transportation safety audits with the **U.S. Department of Transportation** (DOT). By connecting DOT APIs to your agent, you transform complex VIN decoding, safety recall checking, and star rating retrieval into a natural conversation. Your agent can instantly retrieve detailed vehicle specifications from a 17-digit VIN, access the latest NHTSA safety recalls for specific makes and models, and audit official consumer complaints without you ever needing to navigate the comprehensive NHTSA or vPIC portals. Whether you are conducting vehicle history research or coordinating a fleet safety audit, your agent acts as a real-time transportation data coordinator, providing accurate results from a single, authorized source.

### What you can do

- **VIN Orchestration** — Decode any 17-digit VIN to retrieve model year, make, engine specs, and body class.
- **Safety Auditing** — Retrieve official safety recalls and 5-star safety ratings (NCAP) for millions of vehicles.
- **Complaint Monitoring** — Access official consumer complaints filed with NHTSA to identify recurring vehicle issues.
- **Manufacturer Discovery** — List vehicle manufacturers, identify plant locations, and lookup WMI identifiers.
- **Fleet Coordination** — Gather comprehensive technical and safety metadata for entire lists of vehicle makes and models.

### How it works

1. Subscribe to this server
2. Optionally enter your Data.gov API Key for enhanced access
3. Start managing your transportation data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Automotive Researchers & Buyers** — automate the gathering of safety and technical metadata through natural language.
- **Fleet Managers** — coordinate safety audits and recall checks for multiple vehicle types directly from your workspace.
- **Developers** — integrate professional-grade transportation APIs into your AI-driven daily routines.
- **Transportation Advocates** — stay updated with official safety ratings and consumer feedback trends.


## Available Tools (8)
- **decode_vin_details**: Decode Vehicle Identification Number
- **find_wmi_info**: Lookup WMI from VIN
- **get_manufacturer_info**: Get manufacturer details
- **get_safety_recalls**: Check vehicle safety recalls
- **get_types_for_make**: ) produced by a make.

Get vehicle types for make
- **get_vehicle_complaints**: Check owner complaints
- **get_vehicle_safety_ratings**: Get NCAP star ratings
- **list_all_makes**: List vehicle manufacturers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DOT Transportation / 美国交通部** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Decode this VIN: '1FTFW1ED5KFA88210'."

**🤖 AI Agent:**
> I've decoded the VIN. This is a 2019 Ford F-150 with a 3.5L V6 engine and a 4x4 drive system. It was manufactured in the United States. Would you like me to check for any active safety recalls for this model?

---

**👤 You:**
> "Check for safety recalls for a 2022 Tesla Model 3."

**🤖 AI Agent:**
> I've retrieved the recall list for the 2022 Tesla Model 3. There are 2 active recalls, including one related to the 'Autopilot' software and another for the 'Window Automatic Reversal System'. Should I provide the detailed summary for each?

---

**👤 You:**
> "What is the 5-star safety rating for the 2023 Honda CR-V?"

**🤖 AI Agent:**
> According to the NHTSA NCAP ratings, the 2023 Honda CR-V (SUV 4WD) has received an overall safety rating of 5 stars. It scored highly in both frontal and side crash tests. Would you like me to check for any consumer complaints filed for this model?


## ❓ FAQ

**Q: Do I need an API key for the DOT tools?**
Most NHTSA and vPIC APIs are public and do not require a key. However, providing a Data.gov API Key can provide higher rate limits and access to more comprehensive transportation datasets.

**Q: What is a VIN?**
A VIN (Vehicle Identification Number) is a unique 17-digit code used by the automotive industry to identify individual motor vehicles. Decoding it reveals technical specs like the engine type and country of manufacture.

**Q: Can I check for safety recalls using this server?**
Yes! Use the `get_safety_recalls` tool with the vehicle's make, model, and year. Your agent will retrieve the official list of recalls issued by NHTSA for that specific configuration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dot-transportation](https://vinkius.com/mcp/dot-transportation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DOT Transportation / 美国交通部** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dot-transportation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DOT Transportation / 美国交通部** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dot-transportation": {
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
