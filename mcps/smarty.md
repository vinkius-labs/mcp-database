# Smarty MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/smarty)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Equip your AI with enterprise-grade location intelligence to validate, autocomplete, and extract US or International addresses instantly.

## Description
Connect your **Smarty** account to any AI agent and empower your team to sanitize raw address data, query ZIP codes, and format global street locations securely. Interact with powerful geospatial and mailing validation APIs through natural language without writing a single line of custom script.

### What you can do

- **Address Validation (USA/Intl)** — Effortlessly clean and verify messy user inputs calling `validate_us_address`, returning the Delivery Point Validation (DPV)
- **Text Extraction** — Feed your AI unformatted text like emails or notes and run `extract_addresses` to intelligently isolate real physical addresses
- **Autocompletion Tests** — Interrogate the AI dynamically with partial street names using the `autocomplete_us_address` algorithm
- **ZIP Code Checks** — Validate specific 5-digit postal zones using `verify_zip_code` to retrieve associated municipal limits

### How it works

1. Subscribe to this server
2. Enter your Smarty Auth ID and Auth Token
3. Start using Claude, Cursor, or any MCP-compatible client to query your geospatial APIs directly

Stop manually typing test addresses into the Smarty sandbox or setting up Postman. Your AI agent can validate address inputs right inside your coding or chat interface.

### Who is this for?

- **E-Commerce Devs** — test the viability of formatting algorithms by parsing complex address lines dynamically in your IDE
- **Data Engineers** — upload raw customer data lists to your AI and have it extract valid postal locations sequentially
- **Logistics Teams** — quickly verify delivery endpoints for complex multi-unit apartment addresses internally


## Available Tools
- **autocomplete_intl_address**: Predictive autocomplete for international addresses
- **autocomplete_us_address**: Predictive autocomplete for US addresses
- **extract_addresses**: g., emails, documents) and find valid addresses.

Extracts physical addresses from raw text
- **get_account_info**: Retrieves Smarty account information
- **validate_intl_address**: Requires at least the address line and country.

Validates and geocodes an international street address
- **validate_us_address**: Returns delivery point validation (DPV) status and coordinates.

Validates and geocodes a US street address
- **verify_zip_code**: Verifies a ZIP code and returns associated cities and states


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Smarty** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate this US address: 1 Santa Claus Ln, North Pole, AK 99705."

**🤖 AI Agent:**
> I've validated the inputted address using the Smarty API.
**Normalized Result**: 1 Santa Claus Ln, North Pole, AK 99705-9901
**DPV Match**: Yes (Y) - Valid deliverable address
**County**: Fairbanks North Star
**Coordinates**: Latitude 64.75, Longitude -147.34

---

**👤 You:**
> "Can you extract any known addresses from this raw text string: "I live out near the big oak tree at 1600 Amphitheatre Pkwy, Mountain View, CA 94043, come visit soon!""

**🤖 AI Agent:**
> I extracted the following geographic location using the text parsing API:

**Address 1**:
- **Cleaned Line**: 1600 Amphitheatre Pkwy, Mountain View, CA 94043
- **ZIP**: 94043
- **Verification**: Confirmed deliverable (Google Headquarters).

---

**👤 You:**
> "Provide a markdown list of US autocomplete suggestions when a user types "3311 w 300 s s"."

**🤖 AI Agent:**
> Based on the incomplete input `3311 w 300 s s`, the Smarty API returned these 3 most likely completions:

1. **3311 W 300 S**, Salt Lake City, UT 84104
2. **3311 W 300 S**, Syracuse, IN 46567
3. **3311 W 300 S**, Swayzee, IN 46986

Would you like me to run a full DPV validation on the Salt Lake City result?


## ❓ FAQ

**Q: Can the AI find an address hidden inside a block of text automatically?**
Yes! You can paste an entire email string or customer support note into your prompt and ask the AI: 'Extract any addresses mentioned in this text.' The agent triggers the `extract_addresses` engine to return the geolocated and sanitized address format purely.

**Q: How accurate is the address verification?**
Smarty ensures the address is validated against official sources like the USPS using DPV (Delivery Point Validation) for US requests, guaranteeing a package can actually be delivered to the mapped coordinate. Your AI agent returns this rigorous underlying metadata.

**Q: Can I use the agent to fix my dataset dynamically without coding?**
Yes. If you have 20 poorly formatted customer addresses, you can simply paste them in the prompt, asking your AI to 'Run each of these through Smarty and return a markdown table of the normalized addresses.' The agent handles the iteration loop for you via the tools.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/smarty](https://vinkius.com/mcp/smarty)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Smarty** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `smarty` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Smarty** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "smarty": {
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
