# Openli MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openli)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Generate privacy policies, cookie consent banners, and legal compliance documents for your website with automated updates.

## Description
Connect your **Openli** account to any AI agent and take full control of your privacy orchestration and legal compliance through natural conversation. Openli provides a comprehensive platform for managing cookie consent, processing Data Subject Access Requests (DSARs), and maintaining an automated audit trail for your legal agreements.

### What you can do

- **Consent & Agreement Orchestration** — List all published legal agreements programmatically and retrieve detailed version metadata to ensure your terms are always synchronized.
- **Evidence & Audit Intelligence** — Record and save user consent evidence directly from the AI interface to maintain a high-fidelity, legally binding audit trail.
- **DSAR Lifecycle Management** — Access and monitor incoming Data Subject Access Requests via natural language to drive better response times and regulatory compliance.
- **Vendor & Data Processor Control** — List and oversee your organization's third-party vendors and data processors using simple AI commands.
- **Operational Monitoring** — Track system responses and manage privacy audit logs to ensure your compliance workflow is always optimized.

### How it works

1. Subscribe to this server
2. Enter your Openli API Key from your dashboard settings
3. Start managing your privacy hub from Claude, Cursor, or any MCP-compatible client

No more manual spreadsheet tracking for user consent. Your AI acts as a dedicated privacy officer or legal operations assistant.

### Who is this for?

- **Legal & Compliance Teams** — quickly retrieve agreement statuses and monitor audit logs without switching apps.
- **Data Protection Officers (DPOs)** — automate the retrieval of DSAR metadata and track vendor compliance via natural conversation.
- **Product Managers** — streamline the recording of consent evidence directly within the chat interface.


## Available Tools
- **check_openli_status**: Verify connectivity
- **create_agreement**: Create an agreement
- **create_dsar**: Create a DSAR
- **get_agreement**: Get agreement details
- **get_consent**: Get consent details
- **get_dsar**: Get DSAR details
- **get_vendor**: Get vendor details
- **list_agreements**: List agreements
- **list_audit_logs**: List audit logs
- **list_consents**: List consents
- **list_dsars**: List DSARs
- **list_vendors**: List vendors
- **save_consent**: Save consent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Openli** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current legal agreements in Openli."

**🤖 AI Agent:**
> I've retrieved your agreements. You have 3 active documents: 'Privacy Policy', 'Terms of Service', and 'Cookie Policy'. Which one would you like to see the public key for?

---

**👤 You:**
> "Show me all active legal documents that need review before their renewal date."

**🤖 AI Agent:**
> You have 7 legal documents approaching renewal. Your Privacy Policy expires June 30th and requires GDPR Article 13 updates. The Terms of Service for your mobile app need revision by July 15th. 3 cookie consent banners are flagged for reconfiguration due to recent regulatory changes in France and Germany.

---

**👤 You:**
> "Generate a compliance report for my website covering GDPR and cookie consent status."

**🤖 AI Agent:**
> Compliance scan complete for example.com. GDPR status: 89% compliant. Missing items: data processing agreement update and explicit consent for analytics tracking. Cookie consent: 23 cookies detected, 19 properly categorized, 4 require reclassification (2 marketing cookies miscategorized as functional). Overall risk level: Medium.


## ❓ FAQ

**Q: Can my AI automatically find the latest version of my Privacy Policy?**
Yes! Use the `list_agreements` tool. Your agent will respond with complete metadata for all published legal documents, including their unique public keys and last update timestamps in seconds.

**Q: How do I find my Openli API Key?**
Log in to your Openli account, navigate to **Settings** > **API**, and you will find your unique secret API key there.

**Q: Can I use the AI to record consent for a new user?**
Absolutely. Use the `save_consent` tool. Provide the user's email and the public key of the agreement they accepted, and the agent will securely log the evidence in your Openli audit trail.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openli](https://vinkius.com/mcp/openli)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Openli** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `openli` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Openli** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "openli": {
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
