# Rev.com MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/revcom)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate human-powered transcription via Rev.com — manage orders, captions, and file metadata with AI.

## Description
Connect your **Rev.com** account to any AI agent and take full control of your professional transcription and captioning orchestration through natural conversation. Rev.com provides the world's most accurate human-powered media services, and this integration allows you to retrieve order metadata, monitor attachment statuses, and manage professional invoices directly from your chat interface.

### What you can do

- **Order & Service Orchestration** — List all managed orders and retrieve detailed metadata, including creating new transcription or captioning requests programmatically.
- **Attachment & Metadata Control** — Access and monitor file attachments and retrieve detailed technical metadata directly from the AI interface to ensure output quality.
- **Invoice & Financial Intelligence** — Access and list account invoices to maintain a clear overview of your professional service expenses via natural language.
- **Order Lifecycle Management** — Cancel or monitor active orders to ensure your content pipeline is always synchronized.
- **Operational Monitoring** — Track system activity and retrieve user profile metadata using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your Rev.com Client Key and User Key from your developer settings
3. Start managing your professional transcriptions from Claude, Cursor, or any MCP-compatible client

No more manual order checking or searching for captions. Your AI acts as a dedicated media operations manager or content coordinator.

### Who is this for?

- **Media Producers & Journalists** — quickly retrieve transcription statuses and monitor file processing without switching apps.
- **Compliance & Legal Teams** — automate the retrieval of professional invoices and track order history via natural conversation.
- **Operations Managers** — streamline the retrieval of account metadata and monitor organizational media health directly within the chat.


## Available Tools (11)
- **get_user_profile**: com account.

Get current user profile
- **list_attachments**: List attachments for an order
- **list_invoices**: List invoices
- **list_orders**: com orders.

List all transcription and captioning orders
- **cancel_order**: Cancel a pending order
- **create_order**: Create a new transcription or captioning order
- **get_attachment_content**: Get the content of a finished transcript or caption file
- **get_attachment_metadata**: Get metadata of a specific attachment
- **get_invoice**: Get details of a specific invoice
- **get_order**: Get details of a specific order
- **get_order_progress**: Get the progress status of a transcription order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rev.com** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 5 orders in Rev.com."

**🤖 AI Agent:**
> I've retrieved your orders. Your last 5 include 'ORD-9912' (Complete), 'ORD-9913' (In Progress), and three others. Would you like to see the attachments for the in-progress order?

---

**👤 You:**
> "Show me all active transcription and captioning orders with their progress and delivery estimates."

**🤖 AI Agent:**
> 7 active orders. "Board Meeting Recording" (1:42:00): Transcription 78% complete, delivery: today 5 PM. "Product Demo Video" (0:23:00): Captioning in progress, 45% complete, delivery: tomorrow 10 AM. "Podcast Episode 47" (0:58:00): Translation to Spanish, 30% complete, delivery: Wednesday. "Training Series" (3 videos, total 2:15:00): Queued, starts processing in 2 hours. 3 additional caption orders at various stages. Total spend this month: $1,234.

---

**👤 You:**
> "Submit a new transcription order for a 45-minute investor call recording with timestamps."

**🤖 AI Agent:**
> Transcription order created: #ORD-8923. File: investor_call_may13.mp3 (45:12 duration). Service: Human transcription (99%+ accuracy). Options: Timestamps every 30 seconds, speaker identification (2 speakers detected), verbatim transcription. Turnaround: 24 hours (rush available for +50%). Estimated cost: $56.40 ($1.25/min). Output formats: DOCX, TXT, SRT. Order status: Processing. You'll receive an email when the transcript is ready for review.


## ❓ FAQ

**Q: Can my AI automatically find the status and attachments for a specific Rev order?**
Yes! Use the `get_order` and `list_attachments` tools. Your agent will respond with complete metadata, including processing status and links to retrieved files in seconds.

**Q: How do I find my Rev.com Client Key and User Key?**
Log in to your Rev.com account, navigate to the **Settings** or **API** section, and you will find your unique Client Key and User Key there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/revcom](https://vinkius.com/mcp/revcom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rev.com** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `revcom` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rev.com** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "revcom": {
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
