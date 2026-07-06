# Namsor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/namsor-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Detect gender, origin, and ethnicity from names, parse full names, and format phone numbers with AI-powered onomastics.

## Description
Connect **Namsor** to your AI agent to unlock advanced name analysis and data enrichment capabilities. Using sophisticated onomastic algorithms, this server allows you to classify names and validate contact information with high precision.

### What you can do

- **Gender Classification** — Accurately predict if a name is likely male or female based on first and last name data.
- **Origin Detection** — Identify the most probable country of origin (ISO2) for any given name.
- **US Race & Ethnicity** — Classify names according to US Census categories including White, Black, API, and Hispanic.
- **Name Parsing** — Automatically split complex full name strings into structured first and last name components.
- **Phone Formatting** — Validate and format international phone numbers using the context of a person's name.

### How it works

1. Subscribe to this server
2. Enter your Namsor API Key
3. Start enriching your lead data or personalizing communications directly from your AI agent

### Who is this for?

- **Marketing Teams** — Personalize email campaigns by accurately detecting gender and cultural origin.
- **Data Scientists** — Enrich datasets with demographic insights and clean up messy name fields.
- **Sales Operations** — Validate lead information and ensure phone numbers are correctly formatted for global outreach.


## Available Tools (5)
- **parse_name**: Split a full name into its components
- **format_phone**: Format and validate a phone number
- **get_us_race_ethnicity**: Classify a name according to US Census race/ethnicity categories
- **get_gender**: Classify a name as male or female
- **get_origin**: Identify the likely country of origin for a name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Namsor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the likely gender for the name Alex Johnson?"

**🤖 AI Agent:**
> I've analyzed the name. 'Alex Johnson' is classified as likely Male with a high confidence score.

---

**👤 You:**
> "Identify the country of origin for the name 'Satoshi Nakamoto'."

**🤖 AI Agent:**
> Based on the name 'Satoshi Nakamoto', the most likely country of origin is Japan (JP).

---

**👤 You:**
> "Format the phone number 5551234567 for a person named Maria Garcia."

**🤖 AI Agent:**
> I've formatted the number using the context for Maria Garcia. The validated international format is +1 555-123-4567.


## ❓ FAQ

**Q: Can I determine if a name is male or female using this server?**
Yes! Use the `get_gender` tool by providing a first and last name. The AI will return the likely gender along with a confidence score.

**Q: How do I split a full name string into first and last names?**
You can use the `parse_name` tool. Just provide the full name string, and it will return the structured components.

**Q: Does this support US Census race and ethnicity categories?**
Yes, the `get_us_race_ethnicity` tool classifies names into White, Black, Asian/Pacific Islander (API), and Hispanic categories based on US Census data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/namsor-alternative](https://vinkius.com/mcp/namsor-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Namsor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `namsor-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Namsor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "namsor-alternative": {
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
