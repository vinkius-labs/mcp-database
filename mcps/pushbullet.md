# Pushbullet MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pushbullet)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pushbullet-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pushbullet-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Send files, links, and notifications between your phone and computer instantly with universal copy-paste across all devices.

## Description
Connect your **Pushbullet** account to any AI agent and take full control of your cross-device notification and file orchestration through natural conversation. Pushbullet provides a powerful platform for bridging the gap between your phone, tablet, and computer, and this integration allows you to send notes, links, and ephemeral messages directly from your chat interface.

### What you can do

- **Push & Notification Orchestration** — Send instant notes, links, and addresses to individual devices or your entire network programmatically.
- **Device Lifecycle Management** — List all associated devices and retrieve detailed metadata, including creating new device profiles directly from the AI interface.
- **Contact & Subscription Control** — Access and monitor your Pushbullet contacts and channel subscriptions via natural language to keep your communications synchronized.
- **Ephemeral Messaging Intelligence** — Send real-time ephemeral messages for clipboard syncing and SMS bridging using simple AI commands.
- **Operational Monitoring** — Track push history and manage system metadata to ensure your notification workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Pushbullet Access Token from your account settings
3. Start managing your cross-device pushes from Claude, Cursor, or any MCP-compatible client

No more manual copy-pasting between devices or missing mobile notifications. Your AI acts as a dedicated notification manager or device coordinator.

### Who is this for?

- **Power Users & Developers** — quickly send snippets and URLs between development machines and mobile devices without switching apps.
- **Operations Teams** — automate the delivery of system alerts to specific team member devices via natural conversation.
- **Support Coordinators** — streamline the retrieval of contact metadata and monitor device availability directly within the chat.


## Available Tools
- **register_new_device**: g. a script) to receive pushes.

Add a target device
- **send_push_notification**: Send data to devices
- **subscribe_to_channel**: Follow a channel
- **remove_device**: Delete a device
- **remove_push_record**: Delete a push
- **unsubscribe_from_channel**: Unfollow a channel
- **get_api_status**: Check connection
- **list_push_contacts**: List friends
- **list_connected_devices**: List your hardware
- **list_recent_pushes**: Get push history
- **list_channel_subscriptions**: Get channel feeds
- **test_pushbullet_auth**: Verify credentials


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pushbullet** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Push this link to my phone: https://vinkius.com"

**🤖 AI Agent:**
> Sending link... I've pushed 'https://vinkius.com' to your primary device via Pushbullet. Should I also send it to your computer?

---

**👤 You:**
> "Send a push notification to all my devices with a reminder about the team meeting at 3 PM."

**🤖 AI Agent:**
> Push notification sent to all 4 connected devices. Title: "Team Meeting Reminder". Body: "Team sync at 3:00 PM EST in Conference Room B. Agenda: Q2 review, sprint planning." Delivered to: MacBook Pro (instant), iPhone 15 (instant), iPad Air (instant), Windows Desktop (0.3s delay). All devices confirmed receipt. The notification was also mirrored to your Chrome browser extension.

---

**👤 You:**
> "Share this URL across all my devices and send a copy to my colleague james@meridian.io."

**🤖 AI Agent:**
> Link shared successfully. URL: https://docs.example.com/q2-report. Pushed to your 4 devices with preview: "Q2 Revenue Report - Interactive Dashboard". Copy sent to james@meridian.io via Pushbullet channel (delivered in 0.5s). James will see it on his connected devices. You can track if he opened it in your push history. The link was automatically saved to your clipboard on your active MacBook.


## Installation & Usage

To install and use the **Pushbullet** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pushbullet](https://vinkius.com/mcp/pushbullet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
