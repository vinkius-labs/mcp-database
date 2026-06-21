# UKG Pro MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ukg-pro)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ukg-pro-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ukg-pro-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage HR data, employee profiles, and payroll via UKG Pro.

## Description
The UKG Pro MCP Server integrates the Model Context Protocol with the UKG Pro human capital management suite, enabling AI agents to manage HR data, employee profiles, payroll details, and organizational structures seamlessly.


## Available Tools
- **organizations**: List organizational components and structures
- **employees**: Get a specific employee by ID in UKG Pro
- **jobs**: Get a specific job configuration by job code
- **payroll**: Get payroll records for the current pay period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UKG Pro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the contact details for employee ID 12345."

**🤖 AI Agent:**
> Here are the contact details for employee 12345: John Doe, Email: john.doe@example.com...

---

**👤 You:**
> "Show the current organizational reporting structure for the 'Marketing' division."

**🤖 AI Agent:**
> Querying UKG Pro organization charts ('get_org_metrics')...
Marketing Division hierarchy:
- VP of Marketing: Sarah Jenkins
  |- Director of Content: Mark D.
  |- Director of SEO: Alice R.
Total active headcounts beneath VP: 45.

---

**👤 You:**
> "Verify the payroll status for the latest bi-weekly run."

**🤖 AI Agent:**
> Fetching payroll parameters ('get_payroll_status')...
The bi-weekly run (Pay Period: Oct 1 - Oct 15) is 'Completed'. Direct deposits were dispatched successfully on Oct 17. Gross payroll total: $450,210.


## Installation & Usage

To install and use the **UKG Pro** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ukg-pro](https://vinkius.com/mcp/ukg-pro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
