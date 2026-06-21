# Udemy MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/udemy)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/udemy-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/udemy-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [learning-training](../categories/learning-training.md)

Access Udemy API to search courses, retrieve instructor reviews, QA, and messages.

## Description
The Udemy MCP Server brings the world's largest selection of courses into your AI workflows. It allows you to search the public catalog, as well as seamlessly retrieve instructor-specific data like QA interactions, direct messages, and course reviews for deep analysis.


## Available Tools
- **course_reviews**: Provide course ID.

List reviews for a specific public Udemy course
- **instructor_courses**: List all courses taught by the authenticated instructor
- **instructor_messages**: List direct messages for the authenticated instructor
- **instructor_qa**: List QA questions in all courses taught by the authenticated instructor
- **instructor_reviews**: Useful for feedback analysis.

List reviews for all courses taught by the authenticated instructor
- **courses**: Get details of a specific Udemy course by ID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Udemy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find top rated courses about 'React' on Udemy."

**🤖 AI Agent:**
> I will query the Udemy public catalog for the keyword 'React' and process the top results.

---

**👤 You:**
> "Check all my unread direct messages from students on Udemy."

**🤖 AI Agent:**
> I'll fetch your instructor direct messages filtering by unread status.

---

**👤 You:**
> "Summarize the latest reviews left on my instructor courses."

**🤖 AI Agent:**
> Retrieving your recent instructor reviews to give you a sentiment summary.


## Installation & Usage

To install and use the **Udemy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/udemy](https://vinkius.com/mcp/udemy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
