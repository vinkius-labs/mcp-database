# Postal Address Normalizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/postal-address-normalizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Standardizes and validates unstructured postal addresses for US, UK, CA, and AU.

## Description
This MCP server provides high-precision tools to transform messy, human-written address strings into structured, machine-readable data. It handles country-specific abbreviation mapping (e.g., 'Street' to 'ST') and performs strict regex-based validation for postal codes in the US, UK, Canada, and Australia. Use `normalize_address` to decompose raw strings, `validate_postal_code` to verify regional formats, and `evaluate_address_completeness` to calculate a deliverability score based on mandatory field presence.


## Available Tools (3)
- **evaluate_address_completeness**: Determines if an address contains all the necessary components for successful delivery in a specific region
- **normalize_address**: Converts a raw, unstructured address string into a structured and standardized format
- **validate_postal_code**: Checks if a specific postal code string is structurally valid for a given country


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Postal Address Normalizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Normalize this address for the US: 123 Main Street, Springfield, IL 62704"

**🤖 AI Agent:**
> {
  "recipient": null,
  "streetNumber": "123",
  "streetName": "Main",
  "directional": null,
  "suffix": "ST",
  "unit": null,
  "city": "Springfield",
  "stateProvince": "IL",
  "postalCode": "62704",
  "deliverabilityScore": 100
}

---

**👤 You:**
> "Is the postal code M5V 2T6 valid for Canada?"

**🤖 AI Agent:**
> {
  "isValid": true,
  "countryFormatMatch": true,
  "confidenceScore": 1.0
}

---

**👤 You:**
> "Check if this address is complete for Australia: 45 George St, Sydney"

**🤖 AI Agent:**
> {
  "isComplete": false,
  "missingFields": ["postalCode"],
  "completenessScore": 75
}


## ❓ FAQ

**Q: Which countries are supported?**
The server currently supports the United States (US), United Kingdom (UK), Canada (CA), and Australia (AU).

**Q: How is the deliverability score calculated?**
The score is derived from the completeness of mandatory components and how strictly the postal code adheres to the expected regional pattern.

**Q: Can I use this to standardize street suffixes?**
Yes, the `normalize_address` tool automatically applies country-specific abbreviation dictionaries to standardize suffixes like 'Avenue' to 'AVE'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/postal-address-normalizer](https://vinkius.com/ai-agent-connect/postal-address-normalizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Postal Address Normalizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `postal-address-normalizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Postal Address Normalizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "postal-address-normalizer": {
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
