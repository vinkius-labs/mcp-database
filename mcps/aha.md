# Aha! MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aha)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/aha-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/aha-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Product roadmapping and strategy — manage features, ideas, and strategic goals via AI.

## Description
Connect your **Aha!** account to your AI agent to unlock professional product management and roadmap orchestration. From capturing new product ideas to auditing technical metadata for features and tracking strategic initiatives, your agent handles your product lifecycle through natural conversation.

### What you can do

- **Feature Orchestration** — List and retrieve details for features, update statuses, and audit requirement hierarchies
- **Idea Management** — List and create product ideas to ensure customer feedback is always captured and categorized
- **Strategic Oversight** — Monitor high-level goals and initiatives to ensure your team is aligned with the product vision
- **Release Tracking** — Retrieve details on upcoming product releases and associated work items across your portfolios
- **Product Insights** — Quickly identify feature bottlenecks or unvoted ideas directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your Aha! API Key and Subdomain
3. Start managing your product roadmaps and retrieving strategy insights through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — automate feature status updates and monitor roadmap progress effortlessly
- **Product Owners** — audit child requirements and manage backlog ideas on the fly
- **Strategic Planners** — verify initiative alignment and track goal completion patterns
- **Engineering Leads** — quickly look up feature technical metadata and release schedules using simple commands


## Available Tools
- **list_features**: List product features
- **get_feature**: Get feature details
- **list_ideas**: List product ideas
- **create_idea**: Capture a new product idea
- **list_releases**: List product releases


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aha!** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active features in my 'Web App' product."

**🤖 AI Agent:**
> I've retrieved the features for the Web App product. You have 10 features currently in development and 5 in the backlog. Would you like to see the status or due dates for any of them?

---

**👤 You:**
> "Create a new idea named 'Dark Mode Support' with description 'User requested dark theme for better accessibility'."

**🤖 AI Agent:**
> I've successfully created the idea 'Dark Mode Support' in your ideation portal. The idea reference is IDEA-123. Would you like me to check if there are similar ideas already existing?

---

**👤 You:**
> "Show me the details for feature ID 'APP-F-101'."

**🤖 AI Agent:**
> I've retrieved the metadata for feature APP-F-101 (Multi-factor Authentication). It is currently in the 'In Development' stage and is assigned to the 'Security Team'. The target release is 'Q3 Security Update'.


## Installation & Usage

To install and use the **Aha!** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aha](https://vinkius.com/mcp/aha)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
