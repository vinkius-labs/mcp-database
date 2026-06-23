# Sansan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sansan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Digitize and manage business cards via AI — browse contacts, verify details, and explore your company's network effortlessly.

## Description
Connect your **Sansan** account to any AI agent to access your organization’s entire secure network of digitized business cards. Effortlessly manage contact relationships directly from Claude, Cursor, or your preferred MCP client.

### What you can do

- **Business Cards** — List all scanned cards, retrieve comprehensive details by card ID, and search for specific contacts by name
- **Personnel Records** — Browse individual person profiles across all captured cards and access deep contact details
- **Network Organization** — Inspect all available tags used for structuring and organizing business cards
- **Enterprise Structure** — List registered Sansan users and view all distinct departments within your organization

### How it works

1. Subscribe to this server
2. Enter your Sansan API Key
3. Start fetching and organizing contact connections instantly from your AI interface

Turn scattered business cards into a searchable relationship graph controlled by your AI agent.

### Who is this for?

- **Sales Teams** — Instantly retrieve digitized contact information before a call without breaking your CRM workflow
- **Executives** — Search for a specific executive's contact details instantly from past networking events
- **Operations** — Audit company's departmental structures and user accounts quickly


## Available Tools (8)
- **get_biz_card**: Retrieves details for a specific business card
- **get_person**: Retrieves details for a specific contact person
- **list_biz_cards**: Lists all scanned business cards
- **list_departments**: Lists all departments in the organization
- **list_persons**: Lists all contact persons across cards
- **list_tags**: Lists all tags used for organizing business cards
- **list_users**: Lists all Sansan users in the organization
- **search_biz_cards**: Searches for business cards by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sansan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for a business card with the name 'Tanaka'."

**🤖 AI Agent:**
> I searched your database and found 2 business cards matching 'Tanaka'. 1. Hiroshi Tanaka (Director at Widget Corp) 2. Kenji Tanaka (Sales Manager at Acme). Let me know if you need full details for a specific ID.

---

**👤 You:**
> "Can you list all the tag categories in our Sansan database?"

**🤖 AI Agent:**
> Certainly. I retrieved your active tags. You have the following categories: 'VIP', '2025 Tech Summit Leads', 'Vendor', and 'Partner'. We can list contacts attached to any of these.

---

**👤 You:**
> "Get the detailed person profile for the ID 'person-12345'."

**🤖 AI Agent:**
> Here is the detailed profile for person-12345: The contact is Satoshi Nakamoto. Current Title: CEO. Email: satoshi@example.com. Phone: +81 3-1234-5678. The record confirms 3 business cards merging to form this unified profile.


## ❓ FAQ

**Q: Can my AI agent find a specific business card by just a first name?**
Yes. Ask the agent to run the `search_biz_cards` tool with the contact's name. It will look through all digitized cards in the shared corporate database and return the matching profiles, including their company, department, and direct contact details.

**Q: Is it possible to list only contacts from a specific department?**
Yes, you can ask your agent to first execute `list_departments` to view your organizational structure, and then cross-reference those entities with the cards via natural prompts to summarize card acquisitions per department.

**Q: What is the difference between business cards and persons?**
Business Cards are individual scan snapshots of physical cards acquired over time. A 'Person' represents the consolidated identity created when multiple updated cards from the same individual are merged. You can query both views via `list_biz_cards` or `list_persons`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sansan](https://vinkius.com/mcp/sansan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sansan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sansan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sansan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sansan": {
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
