# PreciseFP MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/precisefp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Collect client financial data digitally with compliant intake forms designed for wealth management and financial planning firms.

## Description
Connect your **PreciseFP** account to any AI agent and take full control of your financial planning data orchestration through natural conversation. PreciseFP is the premier platform for data gathering in the wealth management industry, and this integration allows you to retrieve client metadata, monitor engagement progress, and trigger custom 'Fact Finder' forms directly from your chat interface.

### What you can do

- **Account & Client Orchestration** — List all managed client and prospect accounts and retrieve detailed profile metadata programmatically to ensure your onboarding is always synchronized.
- **Person & Profile Intelligence** — Access and monitor individual person records within accounts and create new profiles directly from the AI interface to maintain a high-fidelity database.
- **Engagement & Form Control** — List and trigger form engagements (like tax updates or risk profiles) via natural language to drive better data collection efficiency.
- **Template Discovery** — Access your library of form and PDF templates to ensure you always send the correct data requests to your clients.
- **Operational Monitoring** — Track account activity history and manage engagement metadata using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your PreciseFP Access Token (Bearer Token) from your integration settings
3. Start managing your financial data gathering from Claude, Cursor, or any MCP-compatible client

No more manual status checking or template searching. Your AI acts as a dedicated financial operations assistant or client coordinator.

### Who is this for?

- **Financial Advisors & Wealth Managers** — quickly retrieve client summaries and monitor onboarding progress without switching apps.
- **Operations Teams** — automate the triggering of annual review forms and track completion rates via natural conversation.
- **Support Coordinators** — streamline the retrieval of person metadata and monitor organizational health directly within the chat.


## Available Tools
- **create_form_engagement**: Send a form to a client (Engagement)
- **create_person**: g., co-client, child, beneficiary) within an existing account.

Add a person to an account
- **get_account_activity**: Get activity history for an account
- **get_account**: Get PreciseFP account details
- **get_form_engagement**: Get details for a form engagement
- **get_form_template**: Get form template details
- **get_pdf_template**: Get PDF template details
- **get_person**: Get details for a person
- **list_accounts**: Supports filtering by name or type.

List PreciseFP accounts
- **list_form_engagements**: List recent form engagements
- **list_form_templates**: List available form templates
- **list_pdf_templates**: List available PDF templates
- **list_persons**: List persons in an account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PreciseFP** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active client accounts in PreciseFP."

**🤖 AI Agent:**
> I've retrieved your accounts. You have 45 active clients including 'The Miller Family' and 'Robert Chen'. Would you like to see the recent activity for any of them?

---

**👤 You:**
> "Show me all pending client questionnaires that have not been completed in the last 14 days."

**🤖 AI Agent:**
> 18 questionnaires pending beyond 14 days. 7 are "Financial Planning Intake" forms (average wait: 22 days). 4 are "Risk Assessment" questionnaires. 3 are "Insurance Needs Analysis" (oldest: 34 days from Robert Chen). 4 are "Estate Planning" documents. 6 clients have opened the form but not submitted. Recommended action: send automated reminders to the 12 clients who have not opened their questionnaire at all.

---

**👤 You:**
> "Send the retirement planning questionnaire to the Johnson family with a 7 day deadline."

**🤖 AI Agent:**
> Questionnaire sent successfully. Template: "Retirement Planning Comprehensive". Recipients: Michael Johnson (michael@email.com) and Susan Johnson (susan@email.com). Deadline: May 20, 2025. The form includes 42 fields covering income, assets, liabilities, risk tolerance, and retirement goals. Both recipients received email notifications with secure access links. Auto-reminder emails scheduled for day 3 and day 6.


## ❓ FAQ

**Q: Can my AI automatically find the progress of a specific client engagement?**
Yes! Use the `get_form_engagement` tool with the Engagement ID. Your agent will respond with complete metadata, including completion status and time of the last activity in seconds.

**Q: How do I find my PreciseFP Access Token?**
First, contact PreciseFP support to activate API access. Once enabled, navigate to **Settings** > **Integrations** > **API Tokens** to generate your unique secret token.

**Q: Can I use the AI to see form templates?**
Yes, use the `list_form_templates` tool to retrieve your library of configured forms, allowing the agent to identify which ones to send to your clients.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/precisefp](https://vinkius.com/mcp/precisefp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PreciseFP** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `precisefp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PreciseFP** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "precisefp": {
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
