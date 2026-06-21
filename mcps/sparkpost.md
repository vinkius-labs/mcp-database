# SparkPost MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sparkpost)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sparkpost-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sparkpost-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Bring your SparkPost email delivery platform into your AI. Manage templates, send campaigns, and audit deliverability directly from your editor.

## Description
Connect your **SparkPost** ecosystem natively to your artificial intelligence assistant. Streamline communication workflows by triggering email sending scripts or auditing delivery matrices natively within your code editor. Bypass the need to log into the SparkPost Web UI repeatedly; create intricate newsletter templates using an LLM to generate perfectly formatted HTML arrays and push them dynamically to your SparkPost instance.

### What you can do

- **Transmission Hub** — Use `send_email` to test transactions instantly via standard human prompts
- **Template Factory** — Design and register valid HTML layouts via `create_template`, pulling down raw markup utilizing `get_template_details`
- **Health Monitoring** — Retrieve operational KPIs executing `get_deliverability_metrics`, while simultaneously listing real-time failures by issuing `list_bounce_events`
- **Compliance & Suppressions** — Read exactly who hit the spam or unsubscribe button by commanding `list_suppression_list` and unblocking falsely filtered individuals locally via `delete_suppression_record`

### How it works

1. Subscribe to this AI integration server
2. Provide your overarching SparkPost API Key
3. Engage your language model internally querying about your specific active mailing webhooks

Stop managing HTML string templates manually or debugging mail senders manually in isolated Postman queries. Let the AI understand your Email API context intuitively.

### Who is this for?

- **Developer / Ops** — test transactional emails immediately while scripting local applications without interrupting your workflow
- **Marketing Engineers** — command the bot to parse old templates and refactor HTML layouts directly injecting modernized structures
- **Postmaster Administrators** — audit sudden drops in global metric performance, asking LLMs to filter Bounce Events systematically


## Available Tools
- **create_template**: Provide a unique ID, display name, subject and valid HTML.

Creates a new HTML email template
- **delete_suppression_record**: This action is irreversible.

Removes an email address from the suppression list
- **delete_template**: This action is irreversible.

Permanently deletes an email template
- **get_deliverability_metrics**: Retrieves account-wide deliverability and performance metrics
- **get_template_details**: Retrieves the structure and content of a specific template
- **list_bounce_events**: Lists recent email bounce events
- **list_suppression_list**: g. due to unsubscribes or spam complaints).

Lists addresses on the global suppression list
- **list_templates**: Lists all draft and published email templates
- **list_webhooks**: Lists all active event webhooks
- **send_email**: Provide from_email, to_email, subject and plain text content.

Sends an email via SparkPost transmissions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SparkPost** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check SparkPost metrics and tell me how our overall deliverability looked for the recent period."

**🤖 AI Agent:**
> I've pulled stats via `get_deliverability_metrics`. Your account is looking healthy:
**Total Accepted**: 42,150
**Total Bounced**: 204
**Total Deferred**: 18
**Rejection Rate**: 0.48%

Your bounce rate falls well below the standard 2% danger threshold. Would you like a deeper dump of your `list_bounce_events` nonetheless?

---

**👤 You:**
> "Create a new HTML template titled 'Holiday Promo' using ID 'promo_2025' that features a large header table."

**🤖 AI Agent:**
> I generated a responsive HTML snippet utilizing properly structured centered table bodies. Then, I invoked `create_template` mapping attributes ID `promo_2025` with Name `Holiday Promo` successfully. 

**Result:** The template is now published in your SparkPost account and available for trigger operations immediately.

---

**👤 You:**
> "Send a plain text email to compliance@domain.com saying 'Your account review is ready for audit'."

**🤖 AI Agent:**
> I've invoked `send_email` dynamically setting the headers appropriately to send textual metadata.

**Transmission Result**: SUCCEEDED ✅
Recipient: compliance@domain.com
Subject: Account Review

SparkPost acknowledged the request and the payload is now actively pushing to ISP delivery paths.


## Installation & Usage

To install and use the **SparkPost** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sparkpost](https://vinkius.com/mcp/sparkpost)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
