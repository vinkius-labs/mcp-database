# AWeber MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aweber-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate email marketing via AWeber — manage accounts, mailing lists, and subscribers directly from any AI agent.

## Description
Connect your **AWeber** account to any AI agent to streamline your email marketing workflows. Manage your subscribers and mailing lists through natural conversation.

### What you can do

- **Account Overview** — List all AWeber accounts associated with your access token.
- **List Management** — Retrieve and organize mailing lists for specific accounts.
- **Subscriber Operations** — List, add, and update subscribers within your mailing lists to keep your audience data current.
- **Data Synchronization** — Seamlessly pull subscriber details into your AI's context for better segmentation and analysis.

### How it works

1. Subscribe to this server
2. Enter your AWeber Access Token
3. Start managing your email campaigns from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Email Marketers** — quickly check list growth and subscriber statuses without switching tabs.
- **Sales Teams** — add new leads to specific mailing lists directly from conversation or CRM workflows.
- **Growth Engineers** — automate subscriber updates and list querying within development environments.


## Available Tools
- **list_accounts**: List AWeber accounts
- **add_subscriber**: Add a new subscriber to a list
- **list_lists**: List mailing lists for an account
- **list_subscribers**: List subscribers in a mailing list
- **update_subscriber**: Update an existing subscriber


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AWeber** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my AWeber accounts."

**🤖 AI Agent:**
> I've retrieved your accounts. You have access to 'Main Marketing' (ID: 123456). Would you like to see the mailing lists for this account?

---

**👤 You:**
> "Get the list of subscribers for account 12345 and list 67890."

**🤖 AI Agent:**
> Fetching subscribers for list 67890... I found 150 active subscribers. Would you like me to filter them or export the details?

---

**👤 You:**
> "Add 'john@example.com' with name 'John Doe' to list 67890 in account 12345."

**🤖 AI Agent:**
> Successfully added John Doe (john@example.com) to the mailing list. Their subscriber ID is 998877.


## ❓ FAQ

**Q: Can I add a new subscriber to a specific list using this server?**
Yes! Use the `add_subscriber` tool by providing the account ID, list ID, and the subscriber's email. You can also optionally include their name.

**Q: How do I find the ID for my mailing lists?**
Simply use the `list_lists` tool with your account ID. It will return all mailing lists associated with that account, including their unique IDs.

**Q: Can I update an existing subscriber's information?**
Yes, the `update_subscriber` tool allows you to modify the email or name of an existing subscriber using their unique subscriber ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aweber-alternative](https://vinkius.com/mcp/aweber-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AWeber** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `aweber-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AWeber** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aweber-alternative": {
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
