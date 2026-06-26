# Klaviyo (Marketing Automation) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/klaviyo-marketing-automation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Manage your B2C CRM via Klaviyo — create profiles, track email campaigns, and audit automation flows.

## Description
Connect your **Klaviyo** account to any AI agent and take full control of your e-commerce marketing, customer data, and automation flows through natural conversation.

### What you can do

- **Profile Management** — Create and retrieve detailed customer profiles, including contact information, custom properties, and predictive analytics directly from your agent
- **Campaign Tracking** — List all email campaigns and retrieve detailed performance metadata, targeted audiences, and scheduled send times securely
- **Automation Flows** — Monitor your automated email and SMS sequences, including entry triggers and chronological action steps to ensure your lifecycle marketing is running smoothly
- **Audience Segmentation** — List dynamic segments and static lists to understand your customer distribution and identify high-value cohorts
- **List Orchestration** — Add existing profiles to specific marketing lists to manage subscription preferences and targeted messaging natively
- **Data Audit** — Extract comprehensive traits and behavioral analytics for specific profile IDs to power personalized customer interactions

### How it works

1. Subscribe to this server
2. Enter your Klaviyo Private API Key
3. Start managing your marketing automation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Marketers** — track campaign statuses and audit automation flows through natural conversation without manual dashboard searching
- **Growth Engineers** — verify audience segments and monitor profile custom properties to ensure accurate data mapping
- **Business Owners** — get rapid summaries of recent campaign performances and customer base growth across multiple Klaviyo accounts


## Available Tools (10)
- **get_flow_details**: It returns the entry trigger conditions, the sequence of action steps (emails, SMS, delays), and the current operational status of the automation.

Get details for a Klaviyo automation flow
- **list_audience_segments**: Unlike lists, segments update automatically based on behavioral data and predictive analytics. Use this to understand your high-value customers, churn risks, or engaged subscribers.

List Klaviyo audience segments
- **list_profiles**: This tool is used to browse your customer base and obtain profile IDs, email addresses, and names. Use this as a starting point to find specific customers before performing detailed audits or adding them to lists.

List Klaviyo profiles (contacts)
- **create_profile**: This is essential for manual lead insertion or synchronizing data from other sources. Requires an email address; first and last names are optional but recommended for personalization.

Create a new Klaviyo profile
- **list_lists**: Use this to identify target lists for profile orchestration or to audit your subscription groups. Returns list IDs, names, and total contact counts.

List all Klaviyo audience lists
- **add_profiles_to_list**: This tool is critical for managing subscriptions and segmenting customers for specific marketing campaigns. Input profile IDs as a comma-separated string.

Add profiles to a Klaviyo list
- **list_email_campaigns**: This tool allows you to monitor marketing activity, check which campaigns are currently active, and see scheduled send times for upcoming broadcasts.

List Klaviyo email campaigns
- **get_campaign_details**: Returns its current status (draft, sent, scheduled), the targeted audience list/segment IDs, and the message content being delivered.

Get details for a Klaviyo campaign
- **list_automation_flows**: Use this to audit your automated lifecycle marketing, such as welcome series, abandoned carts, or post-purchase follow-ups. Returns flow IDs, names, and active status.

List Klaviyo automation flows
- **get_profile**: Returns everything from contact info (email, phone, address) to custom e-commerce properties, predictive analytics (CLV, churn risk), and marketing preferences.

Get a Klaviyo profile by ID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Klaviyo (Marketing Automation)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active email campaigns in my Klaviyo account"

**🤖 AI Agent:**
> I've found 3 active campaigns: 'Spring Sale 2024' (ID: camp-123), 'Monthly Newsletter' (ID: camp-456), and 'Product Reveal' (ID: camp-789). Would you like to see the targeted audience or performance metrics for any of these?

---

**👤 You:**
> "Show me the details for automation flow ID 'flow-987'"

**🤖 AI Agent:**
> Retrieving flow 'flow-987' ('Welcome Series')… It is currently ACTIVE. The trigger is 'When someone joins Newsletter'. The sequence includes 3 emails sent over 7 days. Current completion rate is 84%. Would you like to see the individual step details?

---

**👤 You:**
> "Create a profile for 'Sarah Doe' with email 'sarah@example.com'"

**🤖 AI Agent:**
> Profile for Sarah Doe (sarah@example.com) created successfully. ID: prof-012345. I can now add her to your 'New Customers' list or update her profile with custom behavioral properties. What would you like to do next?


## ❓ FAQ

**Q: Can I check the status of an automation flow using my agent?**
Yes. Use the `get_flow_details` tool with a specific Flow ID. Your agent will retrieve the comprehensive status, including entry triggers and the sequence of action steps, allowing you to audit your lifecycle marketing in real-time.

**Q: How do I create a new customer profile through a conversation?**
Use the `create_profile` tool by providing the email address, first name, and last name. Your agent will generate the new contact profile in Klaviyo, ready for segmentation or being added to specific marketing lists.

**Q: Can my agent list all dynamically updated audience segments?**
Absolutely. Use the `list_audience_segments` tool to retrieve all dynamic segments from your Klaviyo account. These segments update automatically based on user behavior and analytics conditions, and your agent can report on their status directly in your chat.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/klaviyo-marketing-automation](https://vinkius.com/mcp/klaviyo-marketing-automation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Klaviyo (Marketing Automation)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `klaviyo-marketing-automation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Klaviyo (Marketing Automation)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "klaviyo-marketing-automation": {
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
