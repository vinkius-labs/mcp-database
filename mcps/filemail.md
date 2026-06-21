# Filemail MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/filemail)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transfer large files up to terabytes securely with password protection, download tracking, and branded transfer pages.

## Description
Connect your **Filemail** account to any AI agent and take full control of your secure file sharing and transfer workflows through natural conversation.

### What you can do

- **Transfer Orchestration** — Initialize large file transfers programmatically and retrieve secure upload URLs and metadata
- **Delivery Tracking** — Monitor sent and received transfers in real-time, including download statuses and expiration dates
- **Asset Access** — Programmatically retrieve download links and compressed ZIP URLs for any transfer in your account
- **Contact Management** — Access your address book and manage recipient directories to streamline your sharing operations
- **System Monitoring** — Track account storage limits, configuration, and API connectivity directly through your agent

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** and **Login Token** from your Filemail account settings
3. Start managing your large file deliveries from Claude, Cursor, or any MCP client

No more manual status checking or complex transfer management through fragmented emails. Your AI acts as your dedicated file logistics coordinator.

### Who is this for?

- **Creative Professionals** — instantly track the delivery of large media assets and manage expiration dates using natural language
- **IT & Ops Leads** — automate file distribution tasks and monitor account storage usage without leaving your workspace
- **Support Teams** — quickly verify if a customer has received a specific transfer and provide direct download links


## Available Tools
- **complete_transfer**: Finalize a file transfer
- **delete_transfer**: Delete a transfer
- **get_configuration**: Get account configuration
- **get_transfer_details**: Get details of a specific transfer
- **get_user**: Get user profile
- **initialize_transfer**: Initialize a new file transfer
- **list_contacts**: List contacts
- **list_received_transfers**: List received transfers (inbox)
- **list_sent_transfers**: List sent transfers
- **login**: Login to Filemail


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Filemail** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my sent transfers on Filemail."

**🤖 AI Agent:**
> I've retrieved your sent transfers. You have 5 active deliveries, including 'Project Alpha Video' (Sent yesterday) and 'Q4 Financials'. Would you like the download status for any of these?

---

**👤 You:**
> "Get the download link for transfer ID 'ABC-123'."

**🤖 AI Agent:**
> Link retrieved! You can download the files for transfer ABC-123 here: [download_url]. The transfer contains 3 files and expires in 7 days.

---

**👤 You:**
> "Check my Filemail account storage usage."

**🤖 AI Agent:**
> Checking storage... You are currently using 45GB of your 100GB total limit. You have 55GB of space available for new transfers.


## ❓ FAQ

**Q: How do I get my Filemail API credentials?**
Log in to your Filemail account, go to account settings, and locate your API Key and Login Token in the developer or security section.

**Q: How do I upload files after initialization?**
This connector handles metadata. Use the 'uploadurl' returned by `initialize_transfer` to upload your file data via your preferred HTTP client.

**Q: Can I check my account storage limits?**
Yes! Use the `get_configuration` tool to retrieve current storage usage, total limits, and account configuration details.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/filemail](https://vinkius.com/mcp/filemail)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Filemail** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `filemail` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Filemail** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "filemail": {
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
