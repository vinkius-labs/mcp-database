# Double the Donation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/double-the-donation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Maximize nonprofit revenue by identifying donors whose employers offer matching gift programs and automating match requests.

## Description
Connect your **Double the Donation** (360MatchPro) account to any AI agent and take full control of your nonprofit matching gift automation and corporate giving workflows through natural conversation.

### What you can do

- **Employer Orchestration** — Search an extensive database of over 24,000 employers programmatically to find specific matching gift opportunities and guidelines
- **Donation Life-cycle** — Programmatically register new donations and automatically identify matching gift eligibility to maximize your fundraising revenue
- **Supporter Tracking** — Access complete status reports for individual donations and monitor the matching gift journey from donor action to payment completion
- **Account Management** — Programmatically provision and manage 360MatchPro accounts for nonprofit clients to streamline your partnership operations
- **Strategic Visibility** — Access high-level dashboard statistics and account settings directly through your agent for instant performance reporting

### How it works

1. Subscribe to this server
2. Retrieve your **Public and Private API Keys** from your 360MatchPro dashboard (Settings > API Keys)
3. Start capturing unclaimed matching gift revenue from Claude, Cursor, or any MCP client

No more manual employer lookups or missing out on corporate gift matches. Your AI acts as your dedicated matching gift coordinator and fundraising strategist.

### Who is this for?

- **Nonprofit Development Teams** — instantly verify employer matching programs and register gifts using natural language commands
- **Fundraising Operations** — monitor donation status across your entire portfolio and track payment completion without leaving your workspace
- **Software Providers** — automate the provisioning of 360MatchPro accounts for your nonprofit clients through simple AI queries


## Available Tools (12)
- **create_organization**: Provision a new 360MatchPro account
- **get_account_settings**: Get account settings
- **get_company**: Get company matching gift details
- **get_dashboard_stats**: Get dashboard statistics
- **get_donation**: Get donation details
- **get_organization**: Get organization details
- **list_campaigns**: List campaigns
- **list_donations**: List donations
- **list_subsidiaries**: List company subsidiaries
- **register_donation**: Register a new donation
- **search_company**: Search for a company by name
- **update_organization**: Update organization details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Double the Donation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'Microsoft' in the employer matching database."

**🤖 AI Agent:**
> Searching database... I found 'Microsoft' (ID: 1024). They have a robust matching gift program with a 1:1 ratio up to $15,000 per employee. Would you like the full guidelines?

---

**👤 You:**
> "Register a $100 donation for 'john.doe@example.com'."

**🤖 AI Agent:**
> Donation registered! I've successfully sent the $100.00 gift from John Doe to 360MatchPro. I'll now monitor the matching eligibility and alert you if an employer is identified.

---

**👤 You:**
> "Get the current matching gift status for donation ID 'don_123'."

**🤖 AI Agent:**
> Fetching status... Donation don_123 is currently in the 'Waiting for Donor' stage. The donor has been notified to submit their matching request. Shall I check for any update emails sent?


## ❓ FAQ

**Q: How do I find my Public and Private API Keys?**
Log in to your 360MatchPro dashboard, navigate to **Settings** > **API Keys**, and copy both your Public and Private access tokens.

**Q: Can I search for any employer in the database?**
Yes! The `search_company` tool allows you to query a database of over 24,000 employers to find matching gift opportunities programmatically.

**Q: Does it support real-time donation status updates?**
The `get_donation` tool retrieves the most current status and history for any registered donation ID directly from the 360MatchPro platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/double-the-donation](https://vinkius.com/mcp/double-the-donation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Double the Donation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `double-the-donation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Double the Donation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "double-the-donation": {
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
