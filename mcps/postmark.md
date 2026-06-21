# Postmark MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/postmark)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/postmark-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/postmark-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Equip your AI to send emails, monitor delivery stats, track bounces, and manage Postmark templates directly from your chat.

## Description
Connect your **Postmark** server safely to any AI agent, granting it the ability to dispatch transactional emails, debug delivery failures, and inspect mailing architectures directly via conversational prompts.

### What you can do

- **Send Emails & Templates** — Command the AI to dispatch text-based emails or trigger rich HTML messages using pre-existing Postmark templates (`send_with_template`)
- **Inspect Bounces & Logs** — Ask why an email failed. The AI can pull exact SMTP traces (`get_bounce_logs`) to explain spam rejections or DNS timeouts
- **Monitor Delivery Stats** — Retrieve precise operational health data, mapping open rates and physical bytes sent across massive volumes
- **Manage Configurations & Templates** — List active webhooks spanning your routing, edit server names, or safely clean up legacy template layouts

### How it works

1. Subscribe to this server
2. Enter your Postmark Server Token
3. Start managing outbound communications natively in Claude, Cursor, or your preferred MCP client

Forget logging into dashboards to copy-paste trace IDs. Ask the model to 'find the latest bounce logs' and watch it dissect the 5xx errors for you.

### Who is this for?

- **Backend Engineers** — quickly check explicit webhook constraints or edit server settings on the fly
- **Support Teams** — investigate exact reasons for "hard bounces" mapping physical UUIDs when users complain about missing emails
- **QA Testers** — effortlessly trigger test templates and read precise delivery confirmation metrics


## Available Tools
- **delete_template**: Delete an email template
- **update_server_config**: Update server name
- **get_bounce_logs**: Get raw SMTP logs for a bounce
- **list_bounces**: List recent email bounces
- **get_delivery_stats**: Get delivery metrics for the server
- **get_server_config**: Get Postmark server configuration
- **list_spam_complaints**: List recent spam complaints
- **list_templates**: List all email templates
- **send_email**: Send a plain text or HTML email
- **send_with_template**: Send an email using a template


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Postmark** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you check if we had any hard bounces yesterday, and tell me why?"

**🤖 AI Agent:**
> I checked `list_bounces`. You had exactly 2 hard bounces related to the `@test.local` domain. Fetching `get_bounce_logs` for UUID `192...`, the upstream MTA rejected it throwing a `550 5.1.1 User Unknown` SMTP code. The inbox genuinely doesn't exist.

---

**👤 You:**
> "List all active Postmark templates, then delete the one clearly named 'Legacy Promo'."

**🤖 AI Agent:**
> Listing your templates... Found 5 active. I have identified 'Legacy Promo' mapped to `template_id` 89321. I'm now invoking `delete_template` on 89321. The layout has been completely purged from your Postmark server.

---

**👤 You:**
> "Send a welcome email through Postmark using template ID `10101` to `user@example.com`."

**🤖 AI Agent:**
> Dispatched gracefully using `send_with_template`. Postmark accepted the request to route template `10101` towards `user@example.com` specifying the sender address `admin@yourdomain.com`. It resolved via message UUID `abc-123`.


## Installation & Usage

To install and use the **Postmark** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/postmark](https://vinkius.com/mcp/postmark)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
