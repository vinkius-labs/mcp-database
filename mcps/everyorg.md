# Every.org MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/everyorg)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Enable donations to over a million nonprofits through a single integration with tax-deductible receipts and giving widgets.

## Description
Connect your **Every.org** account to any AI agent and take full control of your philanthropic discovery and fundraising workflows through natural conversation.

### What you can do

- **Nonprofit Orchestration** — Search across over 1.5 million registered 501(c)(3) nonprofits programmatically using keywords and location filters
- **Cause Intelligence** — Browse and filter nonprofits by specific causes such as climate, education, or animal welfare to maintain high-fidelity social impact
- **Fundraising Automation** — Programmatically create and manage fundraisers for your favorite nonprofits directly through your agent (Requires Private Key)
- **Deep Metadata Retrieval** — Access detailed information for specific nonprofits, including descriptions, EINs, and direct donation links
- **Philanthropic Visibility** — Monitor your active fundraisers and retrieve engagement metadata programmatically using natural language commands

### How it works

1. Subscribe to this server
2. Retrieve your **Public API Key** (and optional **Private Key**) from the Every.org API Dashboard
3. Start discovering nonprofits and managing fundraisers from Claude, Cursor, or any MCP client

No more manual searching through fragmented charity databases. Your AI acts as your dedicated philanthropic coordinator and social impact analyst.

### Who is this for?

- **Social Impact Teams** — instantly identify relevant nonprofits for corporate social responsibility (CSR) initiatives using natural language
- **Fundraisers & Philanthropists** — automate the creation of fundraising campaigns and monitor engagement without leaving your workspace
- **Developers** — integrate high-quality nonprofit data and donation links into custom internal tools and social platforms


## Available Tools
- **browse_by_cause**: Browse by cause
- **browse_causes**: Browse causes
- **check_everyorg_status**: Verify connectivity
- **create_donation**: Create a donation
- **create_fundraiser**: Create a fundraiser
- **get_featured**: Get featured nonprofits
- **get_fundraiser**: Get fundraiser details
- **get_nonprofit_by_ein**: Get nonprofit by EIN
- **get_nonprofit**: Get nonprofit details
- **list_donations**: List donations
- **list_fundraisers**: List fundraisers
- **search_nonprofits**: Search nonprofits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Every.org** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for nonprofits helping with 'ocean cleanup' on Every.org."

**🤖 AI Agent:**
> Searching charities... I've found 5 top-rated nonprofits working on ocean cleanup, including 'The Ocean Cleanup' and 'Surfrider Foundation'. Would you like the direct donation links for any of them?

---

**👤 You:**
> "Browse nonprofits in the 'education' cause."

**🤖 AI Agent:**
> Retrieving education causes... I've found a list of impactful organizations focused on global literacy and STEM education. Notable names include 'Room to Read' and 'Code.org'. Which one should I provide more details for?

---

**👤 You:**
> "Create a fundraiser for 'Room to Read' titled 'Support Global Literacy'."

**🤖 AI Agent:**
> Fundraiser initialized! I've successfully created 'Support Global Literacy' for Room to Read. You can view and share your campaign here: [link]. Your team can now start tracking real-time donations.


## ❓ FAQ

**Q: How do I get an API Key for Every.org?**
Visit the [**Every.org API Dashboard**](https://www.every.org/charity-api) to request your free Public Key. For fundraising features, you will also need a Partner account and Private Key.

**Q: Can I search for nonprofits in a specific location?**
Yes! The `search_nonprofits` tool accepts keywords that can include cities or regions to narrow your search for local organizations.

**Q: How do I create a new fundraiser programmatically?**
Use the `create_fundraiser` tool by providing the `nonprofit_id` (EIN or slug) and a title. Note that this requires a Private Key configured in your credentials.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/everyorg](https://vinkius.com/mcp/everyorg)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Every.org** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `everyorg` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Every.org** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "everyorg": {
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
