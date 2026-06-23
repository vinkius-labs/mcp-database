# Paylocity MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/paylocity)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage payroll and HR via Paylocity — list employees, track earnings, and audit benefits setup directly from any AI agent.

## Description
Connect your **Paylocity** account to any AI agent and take full control of your HR and payroll administration through natural conversation.

### What you can do

- **Workforce Visibility** — List all employees and retrieve detailed profiles, including contact info and job metadata.
- **Earnings & Deductions Tracking** — Inspect specific earning codes and deduction setups for any employee.
- **Onboarding Oversight** — List employees currently in the onboarding process to track hiring progress.
- **Payroll Auditing** — Retrieve local tax configurations, direct deposit settings, and benefit setups to ensure compliance.
- **Custom Data Retrieval** — Access custom fields defined in your Paylocity environment for specific reporting needs.

### How it works

1. Subscribe to this server
2. Enter your Paylocity Client ID, Client Secret, and Company ID
3. Start managing your workforce directly from Claude, Cursor, or any MCP client

### Who is this for?

- **HR Administrators** — quickly lookup employee benefit info or check onboarding status without touching the portal.
- **Payroll Managers** — verify direct deposit or tax configurations for specific employees.
- **Finance Teams** — audit earnings and deductions data for reconciliation tasks.


## Available Tools (10)
- **get_employee_benefit_setup**: Get benefit configuration for an employee
- **get_employee_custom_fields**: Get custom field values for an employee
- **get_employee_deductions**: Get deduction details for an employee
- **get_employee_direct_deposit**: Get direct deposit setup for an employee
- **get_employee_earnings**: Get earning details for an employee
- **get_employee_emergency_contacts**: Get emergency contacts for an employee
- **get_employee**: Get details for a specific employee
- **get_employee_local_taxes**: Get local tax setup for an employee
- **list_employees**: List all employees in the company
- **list_onboarding_employees**: List employees currently in onboarding


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paylocity** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all employees in our company."

**🤖 AI Agent:**
> I've retrieved the employee list. There are 142 employees registered. Would you like to filter by status or search for a specific person?

---

**👤 You:**
> "Show me the earnings and deductions for employee 12345."

**🤖 AI Agent:**
> For employee 12345, earnings include 'Base Salary' and 'Monthly Bonus'. Deductions include 'Health Insurance' and '401k Contribution'.

---

**👤 You:**
> "Who is currently in the onboarding process?"

**🤖 AI Agent:**
> I've fetched the onboarding list. There are 3 employees: 'Alice Brown', 'Michael Scott', and 'Dwight Schrute'. Alice is 80% complete.


## ❓ FAQ

**Q: How do I find my Client ID and Secret?**
You must contact your Paylocity Account Manager or the Paylocity Web Services team to request API credentials. They will provide the Client ID and Client Secret for the WebLink API.

**Q: Where do I get the Company ID?**
Your Company ID is the unique identifier for your organization in Paylocity, typically a 5 or 6 digit number used when logging into the Paylocity portal.

**Q: Can I see an employee's direct deposit setup?**
Yes! Use the `get_employee_direct_deposit` tool with an Employee ID to retrieve the configured bank accounts and distribution settings.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/paylocity](https://vinkius.com/mcp/paylocity)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paylocity** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paylocity` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paylocity** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paylocity": {
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
