# Illumidesk MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/illumidesk)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/illumidesk-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/illumidesk-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage campuses, courses, and users via Illumidesk LMS API.

## Description
Connect your AI agents to Illumidesk, the AI-powered learning management system. This MCP server allows you to list campuses, manage courses, track user memberships, and access activity logs directly through the Illumidesk API. Ideal for automating education workflows and course management.


## Available Tools
- **get_activity_logs**: Retrieves activity logs for a specific campus
- **get_campus**: Retrieves details for a specific campus
- **get_course**: Retrieves details for a specific course
- **get_me**: Gets current authenticated user info
- **list_campuses**: Lists all campuses in Illumidesk
- **list_courses**: Lists all courses within a specific campus
- **list_lti_credentials**: Lists all LTI credentials for a campus
- **list_lti_deployments**: Lists all LTI deployments for a campus
- **list_memberships**: Lists all user memberships in a specific campus
- **list_users**: Lists all users registered in a specific campus


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Illumidesk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all campuses in my Illumidesk account."

**🤖 AI Agent:**
> I'll fetch the list of your Illumidesk campuses.

---

**👤 You:**
> "Show me courses for campus slug 'main-campus'."

**🤖 AI Agent:**
> I'll retrieve the list of courses for that specific campus.

---

**👤 You:**
> "Check who is enrolled in course 'ai-fundamentals'."

**🤖 AI Agent:**
> I'll look up the user memberships for that course.


## Installation & Usage

To install and use the **Illumidesk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/illumidesk](https://vinkius.com/mcp/illumidesk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
