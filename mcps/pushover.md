# Pushover MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pushover)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pushover-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pushover-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate instant push notifications via Pushover — send messages, manage devices, and track delivery with AI.

## Description
Connect your **Pushover** account to any AI agent and take full control of your instant notification orchestration through natural conversation. Pushover provides a simple and robust API for sending real-time alerts to Android, iOS, and desktop devices, and this integration allows you to send messages, verify user tokens, and monitor delivery receipts directly from your chat interface.

### What you can do

- **Notification Orchestration** — Send high-priority alerts with custom sounds, titles, and supplementary URLs programmatically.
- **User & Group Intelligence** — Verify user and group keys to ensure your alerts are always delivered to the correct recipients directly from the AI interface.
- **Receipt & Acknowledgment Control** — Access and monitor delivery receipts for emergency-priority messages to maintain a clear audit trail via natural language.
- **Device & Subscription Oversight** — List associated devices and monitor application limits to ensure your notification pipeline is always optimized.
- **Operational Monitoring** — Track system responses and manage glance data using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your Pushover App Token and User Key from your dashboard
3. Start managing your instant alerts from Claude, Cursor, or any MCP-compatible client

No more manual dashboard testing or complex webhook setups for simple alerts. Your AI acts as a dedicated notification coordinator or operations supervisor.

### Who is this for?

- **DevOps & IT Teams** — quickly send system alerts and monitor incident responses without switching apps.
- **Operations Managers** — automate the delivery of business notifications and track acknowledgments via natural conversation.
- **Power Users** — streamline the retrieval of account limits and monitor multi-device notifications directly within the chat.


## Available Tools
- **grant_app_license**: Assign license to user
- **stop_emergency_alert**: Cancel repeated retries
- **update_glances_data**: Set watch glance info
- **get_message_limits**: Check account quotas
- **get_emergency_receipt**: Check alert status
- **list_registered_devices**: List user hardware
- **list_available_sounds**: Get alert sound names
- **list_user_subscriptions**: List active plans
- **send_emergency_alert**: Send urgent repeated alert
- **send_push_notification**: Send real-time alert
- **test_pushover_auth**: Check connection
- **verify_user_key**: Check user validity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pushover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a high-priority Pushover message: 'Server down in region US-EAST-1'."

**🤖 AI Agent:**
> Sending alert... I've delivered the high-priority notification to your devices via Pushover. Should I check the delivery receipt for you?

---

**👤 You:**
> "Send a critical priority notification to the DevOps team about the production server CPU spike."

**🤖 AI Agent:**
> Emergency notification sent to DevOps group (8 members). Priority: Emergency (requires acknowledgment). Title: "CRITICAL: Production CPU at 94%". Message: "Server prod-web-03 CPU usage spiked to 94% at 2:47 PM. Memory at 87%. Auto-scaling triggered. Immediate investigation required." Sound: persistent alarm. Retry: every 60 seconds until acknowledged. 5 of 8 team members acknowledged within 3 minutes. 3 reminders still active.

---

**👤 You:**
> "Show me the delivery statistics for all notifications sent through Pushover in the last 24 hours."

**🤖 AI Agent:**
> 124 notifications sent in the last 24 hours. Delivery: 121 delivered (97.6%), 2 pending (devices offline), 1 expired (emergency not acknowledged). By priority: 3 emergency, 18 high, 67 normal, 36 low. Top application: "Server Monitoring" with 45 notifications. Peak hour: 2 PM with 14 notifications. Average delivery time: 0.4 seconds. 3 users have exceeded their daily quiet hours limit.


## Installation & Usage

To install and use the **Pushover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pushover](https://vinkius.com/mcp/pushover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
