# Crisp MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crisp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Chat with website visitors in real time, manage support conversations, and build a knowledge base that reduces ticket volume.

## Description
Connect your **Crisp** account to any AI agent and take full control of your multi-channel customer support and visitor engagement workflows through natural conversation.

### What you can do

- **Conversation Orchestration** — List and manage active chat and email support sessions programmatically, including monitoring unread counts and conversation status in real-time
- **Automated Messaging** — Programmatically dispatch text messages to active sessions to coordinate immediate customer assistance and engagement
- **Thread Intelligence** — Access complete message histories for any session to provide high-fidelity context for your support and marketing responses
- **Visitor Lifecycle** — Retrieve detailed visitor profiles and people records to maintain a perfectly coordinated relationship history
- **Operational Monitoring** — Access real-time website traffic metrics and support volume summaries directly through your agent for instant CX reporting

### How it works

1. Subscribe to this server
2. Retrieve your **Plugin ID**, **Plugin Key**, and **Website ID** from the Crisp dashboard
3. Start managing your omnichannel support from Claude, Cursor, or any MCP client

No more manual ticket shuffling or missing messages in busy chat windows. Your AI acts as your dedicated support engineer and visitor engagement coordinator.

### Who is this for?

- **Support Teams** — instantly respond to visitor queries and summarize conversation threads using natural language commands
- **Customer Success** — monitor visitor engagement and retrieve high-fidelity profile metadata without leaving your workspace
- **Growth Marketers** — automate personalized outreach to active visitors and track website traffic through simple AI queries


## Available Tools (6)
- **list_visitors**: List all website visitors/people
- **send_message**: Pass data as a JSON string.

Send a message to a conversation
- **get_conversation**: Get conversation details
- **get_messages**: List messages in a conversation
- **get_visitor_profile**: Get visitor profile details
- **list_conversations**: List all website conversations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crisp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active conversations on my website."

**🤖 AI Agent:**
> I've retrieved your active conversations. You have 3 open chats, including an inquiry from 'John' and a question about 'Premium Features'. Would you like the message history for any of these?

---

**👤 You:**
> "Show the transcript for chat session 'sess_123'."

**🤖 AI Agent:**
> Fetching transcript... Session sess_123 details a discussion about 'Setup Guides'. The visitor requested a link to the documentation, and Agent Sarah replied 10 minutes ago. Shall I draft a follow-up?

---

**👤 You:**
> "Find the visitor profile for 'jane@example.com'."

**🤖 AI Agent:**
> I've located Jane's profile. She has visited the pricing page 3 times today and is currently tagged as a 'VIP Lead'. Would you like to see her full conversation history?


## ❓ FAQ

**Q: How do I find my Crisp API credentials?**
Go to your Crisp dashboard, navigate to the **Marketplace**, create a new plugin, and you will find your Plugin ID and Plugin Key.

**Q: What is the Website ID?**
The Website ID is a unique UUID found in your **Settings** > **Website Settings** section in Crisp.

**Q: Can I retrieve messages from past sessions?**
Yes! The `get_messages` tool allows the agent to retrieve the complete transcript for any session ID in your history.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crisp](https://vinkius.com/mcp/crisp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Crisp** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crisp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Crisp** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crisp": {
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
