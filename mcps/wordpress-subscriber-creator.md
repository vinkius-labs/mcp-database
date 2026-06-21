# WordPress Subscriber Creator MCP Server

This MCP does exactly one thing: it registers a new user in your WordPress database with the strictly enforced 'Subscriber' role. Perfect for turning Claude into an automated lead generation or membership onboarding bot.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/wordpress-subscriber-creator)

## Overview
**Category:** content-management
**Tools Count:** 1

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


## Installation & Usage

To install and use the **WordPress Subscriber Creator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wordpress-subscriber-creator](https://vinkius.com/mcp/wordpress-subscriber-creator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
