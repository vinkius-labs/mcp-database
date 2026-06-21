# Boostapp MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/boostapp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Automate lead management in Boostapp — create new leads, assign pipeline stages, and manage customer data directly from any AI agent.

## Description
Connect your **Boostapp** account to any AI agent to streamline your sales and customer acquisition workflows. This integration allows your AI to act as a virtual sales assistant, capturing lead information and organizing it within your CRM through natural conversation.

### What you can do

- **Lead Creation** — Instantly create new leads with full names and contact numbers directly in the Boostapp system.
- **Pipeline Management** — Automatically assign leads to specific pipeline stages and identify lead sources using system IDs.
- **Detailed Profiling** — Capture comprehensive lead data including email addresses, birth dates, gender, and custom remarks.
- **Subscription Integration** — Link new leads to specific items or subscriptions during the creation process.

### How it works

1. Subscribe to this server
2. Enter your Boostapp API Key
3. Start capturing and managing leads from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Teams** — quickly register leads from conversations or emails without manual data entry.
- **Marketing Managers** — automate the flow of leads from various sources into the CRM pipeline.
- **Business Owners** — maintain a clean and organized customer database using AI-driven automation.


## Available Tools
- **create_lead**: Requires full name and phone number. Can optionally include pipeline stage and subscription details.

Create a new lead in Boostapp


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Boostapp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new lead for John Smith with phone 0501234567 and email john@example.com."

**🤖 AI Agent:**
> I've successfully created the lead for John Smith in Boostapp. The contact is now registered with the provided phone and email.

---

**👤 You:**
> "Add a lead named Sarah Connor, phone 0549876543, and set her pipeline stage to 2."

**🤖 AI Agent:**
> Sarah Connor has been added to Boostapp and assigned to pipeline stage 2.

---

**👤 You:**
> "Register a lead for Mike Ross (0521112233) with the remark 'Interested in the annual subscription' and item ID 101."

**🤖 AI Agent:**
> Done! Mike Ross is now in the system with the note about the annual subscription and linked to item 101.


## ❓ FAQ

**Q: What information is mandatory to create a lead in Boostapp?**
To create a lead using the `create_lead` tool, you must provide at least the `fullName` and a valid `phone` number. All other fields like email or pipeline stage are optional.

**Q: Can I assign a lead to a specific sales stage automatically?**
Yes! When using `create_lead`, you can provide a `stage` ID (number) to place the lead directly into the correct part of your sales pipeline.

**Q: Is it possible to record the source of the lead?**
Absolutely. Use the `leadSource` parameter in the `create_lead` tool to specify the system ID of the marketing or sales source.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/boostapp](https://vinkius.com/mcp/boostapp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Boostapp** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `boostapp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Boostapp** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "boostapp": {
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
