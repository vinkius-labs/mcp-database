# OOPSpam MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/oopspam)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Block spam submissions on your forms and comments with an AI-powered filter that catches bots without annoying real users.

## Description
Connect your **OOPSpam** account to any AI agent and take full control of your content moderation and anti-spam orchestration through natural conversation. OOPSpam provides a privacy-first, highly accurate platform for protecting digital platforms from bots and malicious content, and this integration allows you to retrieve spam scores, monitor usage analytics, and submit manual reports directly from your chat interface.

### What you can do

- **Spam Checking Orchestration** — Instantly analyze text content programmatically to retrieve detailed spam scores and detection reasons without compromising user privacy.
- **Usage & Credit Intelligence** — Access and monitor your account usage statistics and catch-rates directly from the AI interface to ensure your protection is always active.
- **Spam Report Control** — List submitted reports and programmatically report new spam content via natural language to improve your custom filtering logic.
- **Analytical Monitoring** — Retrieve detailed account analytics and track spam trends using simple AI commands.
- **Operational Monitoring** — Track system responses and manage API health to ensure your moderation workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your OOPSpam API Key from your dashboard
3. Start protecting your content from Claude, Cursor, or any MCP-compatible client

No more manual CAPTCHA solving or context switching to moderation dashboards. Your AI acts as a dedicated security analyst or content moderator.

### Who is this for?

- **Community Managers** — quickly retrieve spam scores for user-generated content and monitor community health without switching apps.
- **Compliance & Security Teams** — automate the retrieval of spam analytics and track bot activity via natural conversation.
- **Developers** — integrate real-time anti-spam protection and report submission directly within the chat.


## Available Tools
- **add_blocked_ip**: Block an IP
- **check_bulk**: Bulk spam check
- **check_email**: Check email for spam
- **check_ip**: Check IP for spam
- **check_spam**: Check for spam
- **check_oopspam_status**: Verify connectivity
- **get_analytics**: Get analytics
- **get_daily_stats**: Get daily stats
- **get_stats**: Get usage stats
- **list_blocked_ips**: List blocked IPs
- **list_reports**: List reports
- **submit_report**: Submit spam report


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OOPSpam** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check this message for spam: 'Win a free iPhone now!'"

**🤖 AI Agent:**
> I've analyzed the message. The Spam Score is 5/6, indicating a very high probability of spam. Would you like me to submit a report for this content?

---

**👤 You:**
> "Check if the email address test@tempmail.xyz is likely spam or disposable."

**🤖 AI Agent:**
> The email test@tempmail.xyz has a spam score of 94/100. It was flagged as a disposable email provider. The domain tempmail.xyz is on 3 major blocklists and was registered only 12 days ago. Recommendation: block this email from registration forms to protect your data quality.

---

**👤 You:**
> "Analyze whether the IP address 185.220.101.45 is associated with spam or bot activity."

**🤖 AI Agent:**
> IP 185.220.101.45 has a threat score of 87/100. It is associated with a known Tor exit node in Germany. This IP has been reported 142 times in the last 30 days for automated abuse. It appears on 5 major threat intelligence databases. Recommendation: block or challenge requests from this IP.


## ❓ FAQ

**Q: Can my AI automatically find the spam score for a specific message text?**
Yes! Use the `check_spam` tool. Provide the text content, and your agent will respond with a Spam Score (0-6) and technical detection reasons in seconds.

**Q: How do I find my OOPSpam API Key?**
Log in to your OOPSpam dashboard at oopspam.com, and you will find your unique secret API key displayed in the top right corner of the main page.

**Q: What does a Spam Score of 3 or higher mean?**
A score of 3 or higher generally indicates a high probability that the content is spam. OOPSpam recommends flagging or rejecting content with these scores.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/oopspam](https://vinkius.com/mcp/oopspam)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OOPSpam** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `oopspam` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OOPSpam** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "oopspam": {
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
