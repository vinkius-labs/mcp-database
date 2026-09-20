# Microsoft Outlook MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/microsoft-outlook)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Read, reply, and send Outlook mail plus run your calendar — a full mailbox and scheduling workflow for any AI agent.

## Description
Connect your **Microsoft Outlook** mailbox and calendar to any AI agent through the Microsoft Graph API. Your agent becomes a competent mail and scheduling associate: it can scan your inbox, triage messages, draft and send mail, and manage meetings end to end.

### What you can do

- **Mailbox Triage** — List, search (KQL filters like from: / subject: / unread), and read full messages with attachments metadata
- **Send & Reply** — Compose new mail, reply or reply-all with full conversation context
- **Calendar Control** — List events in any time window, create meetings with attendees, reschedule or cancel them
- **Housekeeping** — Archive or delete messages and events explicitly, one at a time

### How it works

1. Register an Entra application with Microsoft Graph delegated permissions (Mail.Read, Mail.Send, Mail.ReadWrite, Calendar.Read, Calendar.ReadWrite)
2. Subscribe to this server and connect your Outlook account through OAuth 2.0
3. Ask your agent to read, write, and schedule — all inside one mailbox

### Who is this for?

- **Busy Professionals** — delegate inbox triage, follow-up drafting, and meeting management to an agent that never misses a thread
- **Assistants & Coordinators** — run recurring calendar audits and scheduling checks across a shared mailbox workflow


## Available Tools (9)
- **create_calendar_event**: Provide the subject and ISO 8601 start and end times in UTC. Add optional attendees as comma-separated email addresses — they receive an invitation. The created event ID is returned so it can be updated or deleted later.

Schedule a new calendar event
- **delete_calendar_event**: For rescheduling or polite cancellation prefer update_calendar_event with isCanceled. Confirm the event ID with the user before deleting.

Delete a calendar event
- **delete_message**: Use when the user explicitly asks to remove a message. This is not recoverable from the trash by the API — confirm the specific message ID with the user before calling.

Delete an Outlook message permanently
- **list_calendar_events**: Defaults to the next 7 days when no times are given. Provide ISO 8601 datetimes for timeMin and timeMax to target a specific range. Use top to limit how many events are returned in one page.

List calendar events in a time window
- **list_messages**: Use when the user asks to check, scan, or summarize their inbox or another folder. Provide a KQL expression in the query parameter to filter (for example "from:alice" or "subject:invoice AND unread"). Page results with top and skip — a folder never returns everything in one call.

List recent messages from an Outlook mail folder
- **read_message**: Use when the user wants the full text of a message found via list_messages or search. The message ID comes from list_messages results. Add attachments or toRecipients to the select parameter to include those fields.

Read the full content of a specific Outlook message
- **reply_message**: Use when the user wants to answer a message from list_messages or read_message. Set toAll to true for reply-all; otherwise only the original sender is replied to. Provide the message ID of the message being answered.

Reply to an existing Outlook message
- **send_message**: Use when the user asks to draft and send a message. Multiple recipients are comma-separated. Set isHtml to true only when the body contains HTML markup; plain text is the default. Confirm with the user before sending anything with cc recipients.

Send a new email message from the user's Outlook account
- **update_calendar_event**: Use to reschedule, rename, or cancel an event. Canceling by setting isCanceled to true notifies attendees. Provide the event ID from list_calendar_events.

Modify an existing calendar event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Microsoft Outlook** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check my inbox for unread messages from the marketing team and summarize them."

**🤖 AI Agent:**
> Found 4 unread messages from marketing@yoursite.com. 1) The launch page is live as of 09:00, 2) The Q4 budget doc was updated — new cap on paid ads, 3) A meeting invite conflict on Friday was moved to Monday, 4) Two testimonials are ready for the website. Want me to reply to any of them?

---

**👤 You:**
> "Find the 'Q3 forecast' email, open it, and schedule a review with finance@company.com for next Tuesday at 10am UTC."

**🤖 AI Agent:**
> I opened the forecast thread (3 emails, latest from Dana, 12 Sep). Created the event 'Q3 Forecast Review' on your calendar for next Tuesday 10:00–11:00 UTC with finance@company.com invited. The invite is on its way.

---

**👤 You:**
> "Show me today's meetings and cancel the ones after 3pm."

**🤖 AI Agent:**
> You have 5 meetings today. Cancelled: 'Ops sync' (15:30) and 'Vendor call' (16:00) — attendees notified via isCanceled. Keeping: standup, design review, 1:1 with Priya.


## ❓ FAQ

**Q: Which Microsoft Graph permissions does the account need?**
The app registration needs delegated permissions: Mail.Read, Mail.Send, Mail.ReadWrite, Calendar.Read and Calendar.ReadWrite, plus openid/profile/offline_access. You consent once at the OAuth step; the agent then acts strictly on your own mailbox and calendar.

**Q: Does it work with personal Microsoft accounts, or only work/school accounts?**
Both. The OAuth flow uses the multi-tenant common authority, so personal Microsoft accounts and work or school accounts (Microsoft Entra) can connect — the same scopes apply in both cases.

**Q: Can the agent delete a lot of mail at once?**
Deletion is always per-message by explicit ID, never a bulk operation. The agent lists messages first, then deletes one at a time — which keeps the action auditable and reversible only in the way the mailbox itself allows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/microsoft-outlook](https://vinkius.com/en/ai-agent-connect/microsoft-outlook)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Microsoft Outlook** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `microsoft-outlook` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Microsoft Outlook** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "microsoft-outlook": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
