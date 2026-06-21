# SnipForm MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/snipform)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Connect your AI agents to SnipForm to manage form submissions, block spam, handle webhooks, and analyze conversion data.

## Description
Give your AI agents programmatic control over your static site form backend using the SnipForm platform. With 15 precise tools, your AI can automatically review form submissions, manage spam filters, configure webhook integrations, and track conversion analytics in real time.

### What you can do
- List and review all form submissions
- Isolate and manage spam-flagged entries
- Export submission data for external use
- Track per-form analytics and conversion rates
- Configure integrations (Slack, Webhooks, Zapier)
- Create and manage unique form keys

### How it works
1. Subscribe to this server
2. Enter your SnipForm API Key (found in your developer dashboard)
3. Start managing your site forms dynamically via Vinkius

### Who is it for?
Built for frontend developers, marketing teams, and static site operators who need a secure, serverless form backend with powerful AI-driven automation.


## Available Tools
- **check_snipform_status**: Verify connectivity
- **create_key**: Create a form
- **delete_key**: Delete a form
- **delete_submission**: Delete a submission
- **export_submissions**: Export submissions
- **get_account**: Get account info
- **get_form_analytics**: Get form analytics
- **get_key**: Get form details
- **get_submission**: Get submission details
- **list_integrations**: List integrations
- **list_keys**: List all forms
- **list_spam**: List spam submissions
- **list_submissions_by_key**: List submissions by form
- **list_submissions**: List all submissions
- **update_key**: Update a form


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SnipForm** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show the latest form submissions from our primary contact form."

**🤖 AI Agent:**
> I've retrieved the latest 5 submissions for your 'Contact Us' form. The most recent is from 'Jane Doe' regarding an enterprise inquiry. Would you like me to display the full message content?

---

**👤 You:**
> "List all submissions flagged as spam over the last 24 hours."

**🤖 AI Agent:**
> Checking the spam queue... I found 12 submissions blocked by the behavioral filter today. Most appear to be automated bot traffic. Do you want me to list the specific emails or IP addresses involved?

---

**👤 You:**
> "What is the conversion rate and submission volume for our newsletter signup form?"

**🤖 AI Agent:**
> Fetching your form analytics... This month, your 'Newsletter Signup' form has received 450 views and 112 submissions, resulting in a conversion rate of 24.8%. All webhook integrations are currently delivering successfully.


## ❓ FAQ

**Q: How can my AI review recent submissions for a specific contact form?**
Simply use the `list_submissions` tool and provide the form key. Your agent will instantly retrieve all recent entries, including field data and metadata, so you can review inquiries without logging into the SnipForm dashboard.

**Q: Can I automatically check for messages that were blocked by the spam filter?**
Yes. By running the `check_spam_queue` action, your agent can review all submissions flagged by the behavioral scoring system. You can inspect these entries safely to ensure no legitimate messages were falsely identified as spam.

**Q: Is it possible to track the performance and conversion rate of our forms?**
Absolutely. Ask the agent to use the `get_form_analytics` tool. It will compile your submission volume, conversion rates, and integration delivery status over time, giving you a clear view of your lead generation metrics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/snipform](https://vinkius.com/mcp/snipform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SnipForm** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `snipform` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SnipForm** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "snipform": {
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
