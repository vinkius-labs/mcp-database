# WordPress Subscriber Creator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wordpress-subscriber-creator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wordpress-subscriber-creator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wordpress-subscriber-creator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [content-management](../categories/content-management.md)

This MCP does exactly one thing: it registers a new user in your WordPress database with the strictly enforced 'Subscriber' role. Perfect for turning Claude into an automated lead generation or membership onboarding bot.

## Description
We refused to build a bloated WordPress integration that gives an AI agent terrifying access to delete your pages, read your entire database, or install plugins. Instead, this MCP server provides a surgical, zero-trust bridge: **just creating new Subscriber accounts.**

Your AI agent gains the immediate ability to act as a membership onboarding assistant. If a user chats with the AI and says "I want to subscribe to your VIP newsletter", the AI can capture their email and immediately create their account in your WordPress dashboard.

### The Superpowers

- **Zero-Friction Onboarding:** End the manual lead transfer nightmare. The AI registers the user directly via the native WordPress REST API `/wp-json/wp/v2/users`.
- **Compatible with Membership Plugins:** Since it uses the native WordPress user database, this seamlessly integrates with plugins like MemberPress, Restrict Content Pro, or WooCommerce (which treat subscribers as customers).
- **Absolute Containment:** The code is strictly hardcoded to `roles: ['subscriber']`. The AI is physically incapable of creating an Admin or Editor account, ensuring your site remains 100% secure from unauthorized privilege escalation.


## Available Tools
- **create_wordpress_subscriber**: The role is strictly limited to Subscriber, so they have no admin powers. Ideal for member signups, newsletters, or gating content.

Creates a new user account in WordPress with the strictly enforced "subscriber" role


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WordPress Subscriber Creator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Register a new subscriber account for john.doe@example.com with the username johndoe."

**🤖 AI Agent:**
> I've successfully created the subscriber account for johndoe (john.doe@example.com). Their user ID is #125.


## Installation & Usage

To install and use the **WordPress Subscriber Creator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wordpress-subscriber-creator](https://vinkius.com/mcp/wordpress-subscriber-creator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
