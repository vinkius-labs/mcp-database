# Fairing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fairing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Analyze customer insights via Fairing — manage post-purchase surveys, track responses, and query zero-party data through your AI agent.

## Description
Connect your **Fairing** (formerly EnquireLabs) account to any AI agent and take full control of your post-purchase surveys and zero-party data through natural conversation.

### What you can do

- **Survey & Question Management** — List all active questions and fetch detailed configurations for your post-purchase surveys
- **Response Tracking** — List and inspect individual survey responses to understand customer sentiment and attribution
- **Zero-Party Data Analysis** — Query customer-specific responses to pair survey data with your marketing profiles
- **Aggregated Insights** — Extract high-level insights and performance metrics across all your survey streams
- **Integration Audit** — Monitor active integrations with platforms like Klaviyo, GA4, and Meta directly from the cloud
- **Account Context** — Retrieve your Fairing account details and API token identity flawlessly

### How it works

1. Subscribe to this server
2. Enter your Fairing API Key (found in Settings > Account)
3. Start managing your customer insights from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Marketers** — monitor customer attribution and survey performance without leaving your productivity tools
- **Retention Specialists** — review customer-specific feedback to personalize outreach and improve LTV
- **Data Analysts** — pull raw survey responses and insights directly into your AI-powered data workflow


## Available Tools (12)
- **list_surveys**: List all Fairing surveys
- **get_insights**: Get aggregated survey insights
- **get_me**: Get current API token identity
- **get_question**: Get details for a specific survey question
- **get_response**: Get details for a specific survey response
- **get_survey_details**: Get details for a specific survey
- **list_customers**: List customers who have interacted with surveys
- **list_responses**: List all survey responses
- **get_account_info**: Get Fairing account information
- **get_customer_responses**: Get all survey responses for a specific customer
- **list_integrations**: List active Fairing integrations
- **list_questions**: List all Fairing survey questions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fairing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active survey questions on Fairing."

**🤖 AI Agent:**
> I've retrieved your questions. You have 3 active questions including 'How did you hear about us?' (ID: 101) and 'Who is this gift for?' (ID: 102). Would you like to see the response count for any of these?

---

**👤 You:**
> "Show me the latest 5 survey responses."

**🤖 AI Agent:**
> Fetching recent responses... The latest feedback includes 'Instagram Ad', 'Friend Referral', and 'Google Search'. Would you like the details for response ID 205?

---

**👤 You:**
> "Check my active integrations on Fairing."

**🤖 AI Agent:**
> Inspecting integrations... Your account is currently connected to Klaviyo (Syncing), Google Analytics 4 (Active), and Meta (Active).


## ❓ FAQ

**Q: How do I obtain my Fairing API Key?**
You can find your API Key in the Fairing admin portal under **Settings > Account**. Note that API access may depend on your current subscription plan.

**Q: Can I see responses for a specific customer?**
Yes! Use the `get_customer_responses` tool with the specific Customer ID to retrieve all survey feedback associated with that individual.

**Q: What kind of insights can I extract?**
The `get_insights` tool provides aggregated data on question performance, response rates, and attribution trends across your survey streams.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fairing](https://vinkius.com/mcp/fairing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fairing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fairing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fairing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fairing": {
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
