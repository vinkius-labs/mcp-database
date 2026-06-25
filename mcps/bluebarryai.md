# bluebarry.ai MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bluebarryai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Optimize your website accessibility compliance with automated WCAG audits, issue detection, and remediation tracking.

## Description
Connect your **bluebarry.ai** account to any AI agent and take full control of your AI orchestration and multimedia automation workflows through natural conversation.

### What you can do

- **Agent Orchestration** — List and manage all your AI agents programmatically, retrieving detailed status and configuration settings in real-time
- **YouTube Intelligence** — Programmatically analyze and summarize YouTube videos from their URLs using high-fidelity AI processing directly through your agent
- **WhatsApp Automation** — Dispatch automated messages and engage with your audience through official WhatsApp integration to coordinate your digital outreach
- **Automation Monitoring** — Track the status of your active automations across different platforms and retrieve detailed metadata for every process
- **Engagement Architecture** — Access complete directories of your configured AI personas and monitor account-level connectivity for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** (Bearer Token) from your bluebarry.ai dashboard (Account Settings > API)
3. Start orchestrating your AI agents and multimedia tasks from Claude, Cursor, or any MCP client

No more manual toggling between different AI tools or digging through fragmented chat logs. Your AI acts as your dedicated agent engineer and multimedia coordinator.

### Who is this for?

- **Content Creators** — instantly summarize video content and coordinate WhatsApp engagement using natural language commands
- **Marketing Managers** — scale automated outreach and analyze competitor video trends without leaving your workspace
- **Developers** — integrate high-speed AI agent management and video intelligence into custom business workflows through simple AI queries


## Available Tools (6)
- **get_automation_status**: Get status of an automation
- **list_agents**: ai account.

List all AI agents
- **list_automations**: List all active automations
- **send_whatsapp**: ai platform.

Send a WhatsApp message
- **analyze_youtube**: Analyze a YouTube video
- **get_agent**: Get details for an AI agent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **bluebarry.ai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my AI agents in bluebarry.ai."

**🤖 AI Agent:**
> I've retrieved your AI agents. You currently have 5 active personas, including 'Customer Hero' and 'Video Analyst'. Would you like the detailed configuration metadata for any of them?

---

**👤 You:**
> "Analyze and summarize this YouTube video: 'https://youtube.com/watch?v=123'."

**🤖 AI Agent:**
> Processing video intelligence... The summary for the provided video highlights three key technical breakthroughs in model training. Would you like the full high-fidelity transcript summary?

---

**👤 You:**
> "Send a WhatsApp welcome message to '+123456789'."

**🤖 AI Agent:**
> Message dispatched! I've successfully sent the welcome update to +123456789 via bluebarry.ai. The status is currently 'Sent'. Need help monitoring the delivery metadata?


## ❓ FAQ

**Q: How do I find my bluebarry.ai API Key?**
Log in to your account, navigate to **Account Settings** > **API**, and copy your Bearer Token.

**Q: Can I summarize any YouTube video via AI?**
Yes! The `analyze_youtube` tool uses high-fidelity AI to process video URLs and return structured summaries directly to your agent.

**Q: Is the WhatsApp integration official?**
Absolutely. bluebarry.ai uses the official WhatsApp Business API for all automated messaging to ensure high-fidelity delivery.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bluebarryai](https://vinkius.com/mcp/bluebarryai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **bluebarry.ai** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bluebarryai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **bluebarry.ai** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bluebarryai": {
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
