# Rightmove MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rightmove)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Manage Rightmove property listings, track performance metrics, and retrieve branch leads directly through your AI agent.

## Description
Connect your **Rightmove** real-time data feed to any AI agent to streamline your estate agency operations. This server allows you to manage the entire lifecycle of a property listing and monitor its success without leaving your AI interface.

### What you can do

- **Listing Management** — Create new property listings or update existing ones with detailed address, price, and media information using the `send_property` tool.
- **Inventory Control** — Remove properties from the portal using specific reason codes like 'Sold' or 'Withdrawn' via `remove_property`.
- **Lead Retrieval** — Fetch email leads sent by potential buyers or tenants for specific branches over defined periods with `get_branch_emails`.
- **Performance Tracking** — Analyze how your listings are performing with data on search appearances and detail views using `get_property_performance`.

### How it works

1. Subscribe to this server
2. Provide your Rightmove Network ID, Certificate, and Private Key
3. Start managing your property portfolio from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Estate Agents** — Update listings and check leads instantly during client meetings or on the go.
- **Data Analysts** — Pull performance metrics to generate reports on property engagement and market trends.
- **Operations Managers** — Automate the removal of sold properties and sync inventory across platforms efficiently.


## Available Tools
- **get_branch_emails**: Retrieve lead information (emails) for a specific branch
- **get_property_performance**: Retrieve performance statistics for a specific listing
- **remove_property**: Remove a property from the Rightmove website
- **send_property**: If the agent_ref already exists, the property is updated.

Add a new property or update an existing one on Rightmove


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rightmove** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Update the price for property 'REF-998' in branch '12345' to £450,000."

**🤖 AI Agent:**
> I've updated the listing for 'REF-998'. The new price is set to £450,000 with the specified price qualifier. The update has been sent to Rightmove successfully.

---

**👤 You:**
> "Show me the performance stats for property 'AGENT-REF-001' in branch '54321'."

**🤖 AI Agent:**
> For 'AGENT-REF-001', the listing has received 1,240 Search Appearances and 85 Detail Views over the last tracking period. Would you like to see the lead emails for this branch as well?

---

**👤 You:**
> "Remove property 'REF-555' from Rightmove because it was sold."

**🤖 AI Agent:**
> Processing removal for 'REF-555'... I have sent the removal request with reason code 1 (Sold). The property will no longer appear as active on the portal.


## ❓ FAQ

**Q: How do I update the price of an existing property listing?**
Use the `send_property` tool. If you provide an `agent_ref` that already exists in your Rightmove inventory, the system will automatically update the listing with the new `price_info` you provide.

**Q: What information do I get when checking property performance?**
By using the `get_property_performance` tool with a `branch_id` and `agent_ref`, you will receive statistics such as 'Detail Views' (how many people clicked the listing) and 'Search Appearances'.

**Q: Can I specify why a property is being removed?**
Yes. When using the `remove_property` tool, you must provide a `removal_reason` code (for example, 1 for Sold or 2 for Withdrawn) to maintain accurate records on the portal.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rightmove](https://vinkius.com/mcp/rightmove)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rightmove** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `rightmove` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rightmove** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rightmove": {
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
