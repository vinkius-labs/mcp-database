# NumVerify MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/numverify)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Validate and audit phone numbers — identify carriers and locations via AI.

## Description
Empower your AI agent to orchestrate your entire phone validation and identity verification workflow with **NumVerify**, the global API for phone number intelligence. By connecting NumVerify to your agent, you transform complex validation tasks into a natural conversation. Your agent can instantly verify if a number is valid, audit carrier information, and retrieve geographic location data without you ever touching a manual lookup tool. Whether you are cleaning lead lists or verifying user identity, your agent acts as a real-time communications analyst, ensuring your phone data is always verified and accurate.

### What you can do

- **Phone Auditing** — Verify if any international phone number is valid and retrieve detailed metadata, including country and dial codes.
- **Carrier Oversight** — Identify the current carrier for a phone number to maintain a clear view of network distribution.
- **Location Discovery** — Retrieve the geographic location (city/region) associated with a phone number instantly.
- **Line-type Intelligence** — Identify if a number is a mobile, landline, or VoIP line to optimize your communication strategy.
- **Metadata Integrity** — Retrieve official country names and formatting details to maintain strict organizational control over your contact data.

### How it works

1. Subscribe to this server
2. Enter your NumVerify Access Key
3. Start managing your phone intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Operations** — monitor lead lists and retrieve verified phone metadata straight from your workflow.
- **Marketing Managers** — verify if contact numbers are valid and audit carrier distribution for SMS campaigns.
- **Security Teams** — perform rapid audits of user phone numbers and identify line types through natural language.
- **Operations Leads** — automate phone data querying to orchestrate cross-functional communications teams smoothly.


## Available Tools
- **get_phone_line_type**: Identify if a phone number is mobile, landline, or other
- **get_phone_carrier**: Get carrier information for a phone number
- **get_phone_location**: Get geographic location details for a phone number
- **validate_phone**: Verify if a phone number is valid and retrieve metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NumVerify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate the phone number +14158586273 using NumVerify."

**🤖 AI Agent:**
> Phone number validated! The number is valid. It is a mobile line from San Francisco, United States, operated by AT&T. Would you like the full metadata?

---

**👤 You:**
> "Identify the carrier for +442071838750."

**🤖 AI Agent:**
> I've retrieved the carrier information. The number belongs to a landline in London, United Kingdom, and the carrier is identified. Would you like more location details?

---

**👤 You:**
> "Check if +5511999999999 is a mobile line."

**🤖 AI Agent:**
> I've checked the line type. Yes, +5511999999999 is identified as a mobile line in São Paulo, Brazil. I can also retrieve the carrier name if you'd like.


## ❓ FAQ

**Q: How do I find my NumVerify Access Key?**
Log in to your [**NumVerify dashboard**](https://numverify.com/dashboard), and you will find your Access Key on the main page. Copy and paste it below.

**Q: Does it support international numbers?**
Yes. NumVerify covers over 232 countries and provides detailed validation and metadata for global phone numbers.

**Q: Can the agent identify if a number is mobile or landline?**
Yes. The `get_phone_line_type` tool retrieves the line type (e.g., 'mobile', 'landline') allowing you to audit the nature of your contact data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/numverify](https://vinkius.com/mcp/numverify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NumVerify** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `numverify` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NumVerify** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "numverify": {
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
