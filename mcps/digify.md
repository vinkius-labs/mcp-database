# Digify MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/digify)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Equip your AI agent to manage secure files, track data rooms, and monitor document analytics via the Digify API.

## Description
Integrate **Digify**, the leading document security and virtual data room (VDR) platform, directly into your AI workflow. Manage your secure files, monitor data room activity, and track detailed document analytics using natural language.

### What you can do

- **Secure File Oversight** — List and retrieve detailed information and security settings for all your protected files.
- **VDR Management** — Monitor your virtual data rooms, including member lists and collaborative activity.
- **Engagement Analytics** — Retrieve detailed statistics on who viewed your files, for how long, and from where.
- **Access Control** — List recipients and monitor their specific viewing rights and permissions for secure assets.

### How it works

1. Connect the Digify integration to your AI assistant.
2. Authorize using your Digify API Key (found in your account settings).
3. Orchestrate your document security and collaborative research through intuitive conversation.

### Who is this for?

- **Legal & Compliance Teams** — Quickly check who has accessed sensitive documents and their viewing rights on the go.
- **Sales & BD Professionals** — Monitor prospect engagement with sales decks and proposals via chat.
- **Corporate Development** — Manage virtual data rooms and track participant activity during M&A or fundraising.


## Available Tools (10)
- **get_security_account_metadata**: Retrieve metadata and usage limits for your Digify account
- **get_dataroom_details**: Get detailed settings and member lists for a specific data room
- **get_secure_file_details**: Get detailed information and security settings for a specific file
- **get_file_access_statistics**: Retrieve detailed analytics on who viewed your file and for how long
- **quick_file_audit**: Retrieve a high-level summary of file views and security rights
- **list_virtual_datarooms**: List all virtual data rooms (VDRs) in your account
- **list_expired_secure_files**: Identify secure files that have reached their expiration date (mock logic)
- **list_secure_files**: List all secure files you have uploaded to Digify
- **list_file_recipients**: List all people who have been granted access to a specific secure file
- **search_secure_files**: Search for secure files by filename keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Digify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all secure files I've uploaded."

**🤖 AI Agent:**
> I've found 12 secure files in your account, including 'Q3 Financials.pdf' and 'Product Roadmap 2024.docx'. Would you like to see the view count for the most popular one?

---

**👤 You:**
> "Who has viewed the 'M&A Proposal' file and for how long?"

**🤖 AI Agent:**
> The 'M&A Proposal' file has been viewed by 3 people: 'investor1@corp.com' (15 minutes), 'investor2@corp.com' (8 minutes), and 'analyst@firm.com' (45 minutes). Should I check if they have download permissions?

---

**👤 You:**
> "Show me the details for our 'Investor Data Room'."

**🤖 AI Agent:**
> The 'Investor Data Room' contains 45 files and has 8 active members. 5 new documents were added this week. Would you like a list of members who haven't logged in recently?


## ❓ FAQ

**Q: How do I get a Digify API Key?**
Log in to your Digify account, navigate to the API section in your settings, and you can generate or retrieve your unique API Key from there. Note that API access may require a specific plan.

**Q: Can the agent show exactly who viewed a file?**
Yes, you can use the get_file_access_statistics tool to see a list of recipients who have opened your secure file and their total viewing duration.

**Q: Does the integration support watermarking settings?**
The agent can retrieve current security settings for a file, including whether watermarking is enabled. Adjusting these settings should be managed via the Digify dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/digify](https://vinkius.com/mcp/digify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Digify** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `digify` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Digify** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "digify": {
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
