# Custify MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/custify)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Equip your AI agent to manage customer success, monitor health scores, and track churn probability directly via the Custify API.

## Description
Integrate **Custify**, the comprehensive customer success platform, directly into your AI workflow. Monitor customer health, track churn risks, and manage your success tasks and notes using natural language.

### What you can do

- **Customer Oversight** — List and retrieve detailed profiles, health scores, and churn probabilities for all customers.
- **Company Monitoring** — Access company-level metrics and success data to manage B2B relationships effectively.
- **Success Task Management** — List and track open tasks and internal CRM notes for your accounts.
- **KPI Discovery** — Explore key performance indicators and metrics defined in your Custify account.

### How it works

1. Connect the Custify integration to your AI assistant.
2. Authorize using your Custify API Key (found in Settings > API).
3. Optimize your customer success operations through intuitive conversation.

### Who is this for?

- **Customer Success Managers** — Quickly check account health and churn risk on the go.
- **Account Executives** — Retrieve company metrics and recent notes during client reviews.
- **Success Operations** — Audit tasks and KPIs across all customer segments via chat.


## Available Tools
- **create_customer_profile**: Resolves the newly generated customer ID and validation status. Mutates the customer database state.

Create a new customer profile in Custify
- **get_company_details**: Resolves organizational attributes and health metrics. Touches the core company repository.

Get detailed settings and metrics for a specific company
- **get_customer_details**: Resolves health scores, recent activity, and segment membership. Interacts with the behavioral analytics boundary.

Get full profile and health metrics for a specific customer
- **list_companies**: Resolves company IDs, domain information, and association metrics. Touches the account-level organization boundary.

List all companies in Custify
- **list_customers**: Resolves properties such as customer ID, name, email, and lifecycle stage. Interacts with the customer success management boundary.

List all customers in Custify
- **list_customer_kpis**: Resolves metric definitions and threshold values. Interacts with the performance monitoring boundary.

List key performance indicators defined in the account
- **list_customer_notes**: Resolves note content and authorship metadata. Touches the internal communications boundary.

List internal CRM notes for a specific customer
- **list_people**: Resolves contact details and account associations. Touches the relationship management boundary.

List all people associated with accounts
- **list_customer_success_tasks**: Resolves task priority, status, and assigned owners. Interacts with the workflow automation boundary.

List open and completed customer success tasks
- **search_customers_by_keyword**: Resolves matching customer profiles based on name or email. Touches the search and indexing boundary.

Search for customers by name or email


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Custify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all customers with a health score below 50."

**🤖 AI Agent:**
> I've found 8 customers with a health score below 50, including 'Alpha Corp' (Health: 35) and 'Beta Inc' (Health: 42). Both show a high probability of churn. Would you like to see their recent notes?

---

**👤 You:**
> "Show me the success tasks for company 'Alpha Corp'."

**🤖 AI Agent:**
> For 'Alpha Corp', there are 3 open tasks: 'Schedule Q2 Review', 'Update Technical Contact', and 'Follow up on support ticket #123'. One task is overdue. Should I assign these to a specific team member?

---

**👤 You:**
> "Search for customer 'john.doe@example.com'."

**🤖 AI Agent:**
> I found John Doe (john.doe@example.com). He is associated with 'Global Logistics' and has a health score of 82. His churn probability is very low (2%). Would you like to see his full activity history?


## ❓ FAQ

**Q: How do I get a Custify API Key?**
Log in to your Custify account, navigate to **Settings > API**, and you will find your API Key there. Ensure you have the necessary permissions to manage customer data.

**Q: Can the agent update health scores?**
This integration currently focuses on listing and retrieving data. Health scores are typically calculated automatically by Custify based on usage and interaction data.

**Q: Does Custify support B2B company tracking?**
Yes, Custify allows you to track both individual customers and company-level entities, which is fully supported by this integration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/custify](https://vinkius.com/mcp/custify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Custify** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `custify` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Custify** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "custify": {
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
