# Ayrshare MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ayrshare)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ayrshare-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ayrshare-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Social media automation platform — publish posts, schedule content, and track analytics via AI.

## Description
Empower your AI agent to orchestrate your entire social media presence with **Ayrshare**, the powerful automation engine for modern brands. By connecting Ayrshare to your agent, you transform complex multi-platform publishing into a natural conversation. Your agent can instantly publish posts across Twitter, Facebook, Instagram, and LinkedIn, schedule content for optimal reach, audit engagement analytics, and even manage multiple user profiles without you ever opening a browser tab. Whether you're a content creator or a social media manager, your agent acts as a direct bridge to your social networks, ensuring your brand stays active and data-driven.

### What you can do

- **Multi-Platform Publishing** — Publish posts immediately to multiple social networks including text and media attachments via natural language.
- **Content Scheduling** — Schedule future posts with precision timestamps or manage auto-schedule queues for consistent presence.
- **Engagement Analytics** — Retrieve detailed engagement metrics for specific posts or get high-level social profile analytics.
- **Profile Management** — Create, list, and manage different user profiles to organize content across various brands or clients.
- **History Auditing** — Audit your post history to track statuses (Success, Pending, Error) and verify delivery across all channels.

### How it works

1. Subscribe to this server
2. Enter your Ayrshare API Key
3. Start managing your social media presence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Social Media Managers** — automate multi-channel posting and monitor engagement metrics through natural conversation.
- **Content Creators** — schedule posts and retrieve performance data without manual dashboard data entry.
- **Marketing Agencies** — manage multiple client profiles and audit post history efficiently from a single chat interface.
- **Growth Hackers** — integrate social media capabilities into AI-driven marketing workflows for rapid experimentation.


## Available Tools
- **create_post**: Publish a post immediately to social media platforms
- **create_profile**: Create a new user profile
- **delete_auto_schedule**: Delete auto-schedule for a platform
- **delete_profile**: Delete a user profile
- **get_account_check**: Verify Ayrshare connection
- **get_post_analytics**: Get engagement statistics for a specific post
- **get_social_analytics**: Get profile-level analytics for a specific social network
- **list_auto_schedules**: List all auto-schedule settings
- **list_history**: List history of posts
- **list_profiles**: List all user profiles
- **schedule_post**: Schedule a post for a future date
- **set_auto_schedule**: Set auto-schedule times for a platform


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ayrshare** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Publish 'Hello World!' to Twitter and Facebook immediately."

**🤖 AI Agent:**
> I've published your post to Twitter and Facebook. The post is now live, and you can track its performance using the Post ID: `post_abc123`.

---

**👤 You:**
> "Schedule a post for next Monday at 10 AM: 'Join our webinar!' with the image https://example.com/webinar.png"

**🤖 AI Agent:**
> I've scheduled your post and attached the media file for next Monday at 10:00 AM UTC. It will be sent to your primary Twitter profile.

---

**👤 You:**
> "Show me the analytics for my last Instagram post."

**🤖 AI Agent:**
> Retrieving Instagram analytics... Your last post received 150 likes, 12 comments, and reached 1,200 unique accounts. Would you like a more detailed breakdown?


## Installation & Usage

To install and use the **Ayrshare** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ayrshare](https://vinkius.com/mcp/ayrshare)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
