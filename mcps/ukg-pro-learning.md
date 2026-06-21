# UKG Pro Learning MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ukg-pro-learning)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ukg-pro-learning-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ukg-pro-learning-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage employee training, courses, and learning paths via UKG Pro Learning.

## Description
The UKG Pro Learning MCP Server integrates the Model Context Protocol with the UKG LMS, enabling AI agents to query training catalogs, track employee course completions, manage learning paths, and fetch enrollment data.


## Available Tools
- **enrollments**: List enrollments for a specific user
- **courses**: Get a specific training course by ID
- **curricula**: List tracking curricula (Learning Paths)
- **users**: Get details for a specific user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UKG Pro Learning** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active training courses available to the Sales team."

**🤖 AI Agent:**
> Here are the active courses for the Sales team: 1) Advanced Negotiation Skills, 2) Sales Process Overview...

---

**👤 You:**
> "Check the training completion status for employee 'Jane Smith' on the compliance path."

**🤖 AI Agent:**
> Querying UKG Learning records ('get_user_progress')...
Jane Smith (ID: 8841) has completed 80% of the '2026 Annual Compliance' path. 
Remaining modules: 'Data Privacy Basics'.

---

**👤 You:**
> "Assign the 'Cybersecurity 101' curriculum to all new hires in the Engineering department."

**🤖 AI Agent:**
> Executing `assign_curriculum`... Successfully enrolled 12 new Engineering hires into 'Cybersecurity 101' (Curriculum ID: 4022). Due date set for 30 days from today.


## Installation & Usage

To install and use the **UKG Pro Learning** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ukg-pro-learning](https://vinkius.com/mcp/ukg-pro-learning)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
