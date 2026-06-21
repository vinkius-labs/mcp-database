# Enrich CRM MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/enrich-crm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Enhance your CRM records with verified company data, technographic signals, and contact enrichment that keeps your database fresh.

## Description
Connect your **Enrich CRM** account to any AI agent to streamline your B2B intelligence and sales automation workflows through natural conversation.

### What you can do

- **Company Orchestration** — Retrieve detailed firmographics, technical stacks, and financial data using only a company domain programmatically
- **Person Enrichment** — Access professional backgrounds, verified emails, and direct phone lines for your target prospects to maintain a high-fidelity database
- **Email Discovery** — Programmatically find and verify professional email addresses using name and domain combinations directly through your agent
- **Phone Intelligence** — Retrieve direct phone lines to bypass switchboards and reach decision-makers faster
- **Account Visibility** — Monitor your remaining credits and subscription status directly through your agent for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **Enrich CRM API Key** from your dashboard settings
3. Start enriching your sales records and finding new leads from Claude, Cursor, or any MCP client

No more manual contact research or toggling between dozens of browser tabs. Your AI acts as your dedicated B2B data analyst and sales coordinator.

### Who is this for?

- **Sales Development (SDRs)** — build highly targeted outreach lists with verified contact info using natural language commands
- **Marketing Operations** — automate the enrichment of inbound leads for better segmentation and routing without leaving your workspace
- **Growth Engineers** — automate data collection for competitive analysis and technical market research through simple AI queries


## Available Tools
- **enrich_company**: Enrich company data
- **enrich_person**: Enrich person data
- **find_email**: Find a professional email address
- **find_phone**: Find a professional phone number
- **get_account_info**: Check account status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enrich CRM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Enrich the company with domain 'google.com' using Enrich CRM."

**🤖 AI Agent:**
> Company enriched! Google is a 'Technology' giant with 100,000+ employees. Their tech stack includes Kubernetes, TensorFlow, and React. Would you like the detailed financial metadata for their HQ?

---

**👤 You:**
> "Find the professional email for 'Satya Nadella' at 'microsoft.com'."

**🤖 AI Agent:**
> I've found and verified the email for Satya Nadella. The professional address is 'satya@microsoft.com' with a 95% deliverability score. Shall I search for their direct phone line as well?

---

**👤 You:**
> "Check my remaining enrichment credits."

**🤖 AI Agent:**
> You currently have 5,420 enrichment credits remaining in your account. Your subscription plan is active and in good standing. Need help finding more leads?


## ❓ FAQ

**Q: How do I get my Enrich CRM API Key?**
Log in to your Enrich CRM dashboard, navigate to **Settings** > **API**, and copy your unique access token.

**Q: What data points are included in company enrichment?**
You get 250+ technical and financial data points, including tech stack details, employee counts, and HQ location metadata.

**Q: Can I find a phone number using a LinkedIn URL?**
Yes! The `find_phone` tool allows you to provide a LinkedIn profile URL to retrieve associated professional phone lines programmatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/enrich-crm](https://vinkius.com/mcp/enrich-crm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enrich CRM** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `enrich-crm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enrich CRM** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enrich-crm": {
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
