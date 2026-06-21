# Gmail MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gmail)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gmail-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gmail-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your inbox from AI — read, search, organize, and reply to emails across your Gmail efficiently.

## Description
Connect your **Gmail** enterprise or personal account to any AI agent and bring the power of automated email handling into your IDE or chat client.

### What you can do

- **Inbox Reading** — Read full threads, extract important updates, or summarize chains spanning massive email chains completely headless
- **Searching & Filtering** — Run advanced queries (like 'from:boss@company.com is:unread') to zero in on the messages that matter right now
- **Mail Composition** — Draft, formulate, and definitively send responsive emails directly into ongoing threads naturally
- **Label Management** — Categorize, label, organize and modify read/unread states of specific incoming messages to keep Inbox Zero

### How it works

1. Subscribe to this server
2. Supply your OAuth credentials linking to Google Workspace
3. Chat seamlessly through Claude, Cursor, or any MCP client

### Who is this for?

- **Engineers** — extract monitoring alerts and read pull request mails without ever leaving your IDE environment
- **Marketers & PR** — draft hyper-personalized outbound messages and review drafts directly from prompt contexts
- **Operations** — instantly parse huge influxes of updates to find isolated context files and act upon them immediately


## Available Tools
- **batch_delete_messages**: This is NOT reversible — messages cannot be recovered. Use trash instead for safe deletion.

Permanently delete multiple messages
- **create_inbox_filter**: Criteria fields: from, to, subject, query, hasAttachment, negatedQuery. Action fields: addLabelIds, removeLabelIds, forward, star, markImportant. Provide criteria and action as JSON strings.

Create an inbox filter rule
- **list_mailbox_history**: Get the starting history ID from get_gmail_profile. Useful for incremental sync and change detection.

Track mailbox changes since a point in time
- **list_gmail_messages**: Use the "q" parameter for Gmail search syntax (e.g. "from:boss@company.com is:unread", "has:attachment", "newer_than:2d"). Returns message IDs and thread IDs — use get_message_content to read full details.

List messages from the inbox
- **get_message_content**: Use after list_gmail_messages to read specific emails.

Read the full content of an email
- **send_email**: Supports plain text and HTML body, CC, BCC, and reply threading via inReplyTo/references headers. The email is sent immediately.

Compose and send an email
- **send_draft**: The draft is removed after sending.

Send an existing draft
- **get_attachment**: Returns base64-encoded data and size. First use get_message_content to find attachment IDs in the message payload parts.

Download an email attachment
- **modify_message_labels**: Use label IDs (e.g. "UNREAD", "STARRED", "INBOX", or custom label IDs from list_mailbox_labels). Removing "UNREAD" marks as read.

Add or remove labels from a message
- **trash_gmail_message**: Messages in trash are auto-deleted after 30 days. Use untrash_gmail_message to recover.

Move a message to the trash
- **untrash_gmail_message**: Recover a message from the trash
- **batch_modify_messages**: Useful for bulk operations like "mark all as read" (remove UNREAD) or "archive all" (remove INBOX). Provide message IDs as a JSON array string.

Bulk-modify labels on multiple messages
- **list_gmail_threads**: Supports Gmail search syntax via "q". Threads group related messages together.

List conversation threads
- **get_thread_details**: Returns the complete email chain with headers, bodies, and metadata for each message.

Read all messages in a thread
- **list_mailbox_labels**: System labels include INBOX, SENT, TRASH, SPAM, STARRED, UNREAD, IMPORTANT, etc. Use label IDs when modifying message labels.

List all labels in the mailbox
- **get_label_details**: Get details about a specific label
- **create_label**: Labels act as tags — one message can have multiple labels. Use list_mailbox_labels to see existing labels before creating duplicates.

Create a custom label
- **delete_label**: System labels (INBOX, SENT, etc.) cannot be deleted. This is not reversible.

Delete a label permanently
- **list_drafts**: Returns draft IDs and attached message snippets. Use get_draft for full content or send_draft to dispatch.

List email drafts
- **get_draft**: Use this to review a draft before sending.

Read a specific draft
- **create_draft**: The user can review and modify the draft in Gmail or send it later using send_draft. Safer than sending directly.

Create an email draft
- **update_draft**: The draft ID is required — get it from list_drafts.

Edit an existing draft
- **delete_draft**: This is not reversible.

Delete a draft permanently
- **get_vacation_settings**: Check vacation auto-responder status
- **update_vacation_settings**: Optionally restrict to contacts only or domain members. Dates are Unix timestamps in milliseconds.

Toggle vacation auto-responder
- **list_inbox_filters**: Filters automatically process incoming messages based on criteria (from, to, subject, query) and perform actions (add/remove labels, forward, archive, etc.).

List inbox filter rules
- **get_gmail_profile**: Use historyId with list_mailbox_history for change tracking.

Get mailbox identity and stats
- **verify_api_connection**: Check Gmail API connectivity
- **list_unread_emails**: Equivalent to searching with "is:unread".

List the latest unread messages
- **find_emails_from_sender**: Shortcut for the "from:" Gmail search operator.

Search emails by sender address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gmail** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the 3 most recent unread emails from the CEO regarding "Budget"."

**🤖 AI Agent:**
> Searching with "is:unread from:ceo@company.com subject:Budget"... I found two matches: "Budget Revisions 2026" and "Immediate Review: Budget Cuts". Would you like to read the first one?

---

**👤 You:**
> "Send an email to mark@domain.com saying the project is delayed and we need to schedule a call."

**🤖 AI Agent:**
> Email dispatched! Subject dynamically configured to: "Project Update & Call Scheduling". The payload to mark@domain.com confirms the delay and suggests alternative calendar links.

---

**👤 You:**
> "Mark all messages matching 'Promotions 2022' as read in my backend."

**🤖 AI Agent:**
> Successfully filtered 14 emails inside standard promotions and altered their flags globally to 'read'. The inbox footprint is clean.


## Installation & Usage

To install and use the **Gmail** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gmail](https://vinkius.com/mcp/gmail)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
