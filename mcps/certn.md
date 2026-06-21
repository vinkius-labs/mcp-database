# Certn MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/certn)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Automate background checks and screenings for HR and Property Management via Certn — invite applicants, run quickscreens, and retrieve reports.

## Description
Connect your **Certn** account to any AI agent to streamline your background screening processes for both Human Resources and Property Management through natural conversation.

### What you can do

- **HR Screening** — Invite applicants via email/SMS for background checks or run instant 'Quickscreen' checks if you already have consent.
- **Report Management** — Retrieve detailed reports in PDF, HTML, or via secure hosted links valid for one hour.
- **Property Management** — Manage tenant screenings, create property listings, and track applicant statuses for real estate workflows.
- **Package & Team Oversight** — List available screening packages, manage teams, and view user access across your organization.
- **Comprehensive Checks** — Request specific checks including Criminal Record Checks (CRC), Credit Checks, Identity Verification, and Right to Work.

### How it works

1. Subscribe to this server
2. Enter your Certn Client ID and Client Secret
3. Start managing screenings from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HR Managers & Recruiters** — Send screening invites and check candidate statuses without leaving your communication tools.
- **Property Managers** — Streamline tenant applications and property listings directly through your AI assistant.
- **Compliance Officers** — Quickly access background check reports and verify identity documentation for audit purposes.


## Available Tools (18)
- **add_hr_packages**: Add checks to an existing HR application
- **create_pm_property**: Create a new property
- **get_hr_applicant**: Retrieve details/status of a specific HR application
- **get_hr_report_link**: Create a hosted PDF link for an HR report (valid for 1 hour)
- **get_hr_report_pdf**: Download HR report as PDF
- **get_hr_report_web**: Download HR report as HTML
- **invite_hr_application**: Invite an HR applicant via email/SMS
- **invite_pm_application**: Invite a tenant via email for Property Management
- **list_hr_applicants**: List all HR applications
- **list_listings**: List all rental listings
- **list_packages**: List background check packages
- **list_pm_applicants**: List all PM applications
- **list_pm_properties**: List all properties
- **list_superteams**: List superteams
- **list_teams**: List teams
- **list_users**: List users
- **quick_hr_application**: Screen an HR applicant instantly (Quickscreen)
- **quick_pm_application**: Screen a tenant instantly for Property Management


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Certn** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all current HR applicants and their statuses."

**🤖 AI Agent:**
> I've retrieved the list of HR applications. You have 3 pending (John Doe, Jane Smith) and 5 completed reports. Would you like to see the details for a specific applicant?

---

**👤 You:**
> "Invite a new applicant for HR screening: John Doe (john.doe@email.com)."

**🤖 AI Agent:**
> Invitation sent! John Doe has been invited via email to complete their background check application. The Application ID is 'hr_app_98765'.

---

**👤 You:**
> "Download the PDF report for applicant ID 550e8400."

**🤖 AI Agent:**
> I've generated the PDF report for applicant 550e8400. You can access the document here: [Link].


## ❓ FAQ

**Q: Can I instantly screen an applicant if I already have their data and consent?**
Yes! Use the `quick_hr_application` or `quick_pm_application` tools. These allow you to submit all applicant information and consent proof immediately for instant processing.

**Q: How do I get a shareable link for a background check report?**
You can use the `get_hr_report_link` tool. It generates a hosted PDF link for a specific report ID that remains valid for one hour.

**Q: Can I add more checks to an application that has already been submitted?**
Yes, the `add_hr_packages` tool allows you to append additional background checks (like credit checks or criminal records) to an existing applicant ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/certn](https://vinkius.com/mcp/certn)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Certn** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `certn` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Certn** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "certn": {
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
