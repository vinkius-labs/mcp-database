# Culture Amp MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/culture-amp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to manage employee engagement surveys, monitor performance, and track development via the Culture Amp API.

## Description
Integrate **Culture Amp**, the leading employee experience platform, directly into your AI workflow. Monitor organizational health, track engagement survey progress, and manage employee data using natural language.

### What you can do

- **Employee Management** — List and retrieve detailed profiles for all employees in the platform.
- **Engagement Insights** — Monitor active and past engagement surveys and their participation status.
- **Organizational Structure** — Explore teams and groups defined within Culture Amp to understand your company layout.
- **Analytics Discovery** — List available analytics datasets and demographics for reporting segmentation.

### How it works

1. Connect the Culture Amp integration to your AI assistant.
2. Authorize using your Culture Amp API Key (found in your organization settings).
3. Optimize your employee experience strategy through intuitive conversation.

### Who is this for?

- **People & HR Operations** — Quickly audit employee records and monitor survey participation rates.
- **Team Leads** — Retrieve team-specific data and track engagement trends within their departments.
- **Internal Communications** — Identify engagement gaps and plan outreach based on real-time survey status.


## Available Tools (10)
- **create_employee_record**: Resolves newly created user IDs and verification status. Mutates the employee directory state.

Add a new employee to the Culture Amp platform
- **get_survey_details**: Resolves participant counts and survey settings. Touches the analytics data-source boundary.

Get configuration and status for a specific survey
- **get_employee_details**: Resolves full profile attributes. Touches the core employee information system.

Get detailed profile for a specific employee
- **list_cultureamp_accounts**: Resolves account IDs and organizational scopes. Touches the account management boundary.

List accounts associated with your organization
- **list_analytics_datasets**: Resolves dataset identifiers and types. Touches the reporting data-warehouse boundary.

List available analytics datasets for reporting
- **list_demographic_fields**: Resolves demographic field names and identifiers. Touches the metadata and segmentation boundary.

List demographics used for reporting segments
- **list_organizational_groups**: Resolves group IDs, names, and hierarchical classifications. Touches the organizational mapping boundary.

List groups and teams defined in Culture Amp
- **list_engagement_surveys**: Resolves survey IDs, titles, and lifecycle statuses (active, closed). Interacts with the feedback analytics boundary.

List all engagement and experience surveys
- **list_employees**: Resolves properties such as user ID, email, and employee status. Interacts with the employee directory boundary.

List all employees in Culture Amp
- **search_employees_by_name**: Resolves matched employee profiles. Touches the search and discovery boundary.

Search for employees by name or email keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Culture Amp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all employees in the 'Engineering' team."

**🤖 AI Agent:**
> I've retrieved 25 employees from the Engineering team, including 'John Smith', 'Jane Doe', and 'Mike Ross'. Would you like to see the profile for any of them?

---

**👤 You:**
> "What is the participation rate for our current 'Annual Engagement' survey?"

**🤖 AI Agent:**
> The 'Annual Engagement' survey currently has a 75% participation rate, with 450 out of 600 employees responded. 5 days remain until the survey closes. Should I check which departments have lower participation?

---

**👤 You:**
> "Show me the organizational groups defined in our account."

**🤖 AI Agent:**
> I've found 15 organizational groups, including 'Management', 'Sales North America', 'London Office', and 'Product Design'. Which group would you like to explore further?


## ❓ FAQ

**Q: How do I get a Culture Amp API Key?**
Log in to Culture Amp as an administrator, navigate to **Settings > Data Integrations**, and you will find the API section to generate a new key.

**Q: Can I see individual survey responses?**
To protect employee anonymity, the API generally provides aggregated survey data and participation status, rather than individual identifiable responses.

**Q: Does the integration support demographic segmentation?**
Yes, you can use the list_demographic_fields tool to view how your data is segmented, allowing the agent to provide more targeted insights.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/culture-amp](https://vinkius.com/mcp/culture-amp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Culture Amp** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `culture-amp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Culture Amp** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "culture-amp": {
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
