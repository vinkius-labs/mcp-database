# Unanet MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/unanet)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/unanet-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/unanet-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Project-based ERP for government contractors and professional services.

## Description
The Unanet MCP Server connects AI agents to the Unanet project management and ERP suite. It enables agents to read timesheets, view expense reports, query project statuses, and list organizational workforce data, streamlining compliance and operational efficiency.


## Available Tools
- **expenses**: List expense reports for a user
- **projects**: List projects in Unanet
- **timesheets**: List timesheets for a user
- **users**: List users/employees in Unanet


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Unanet** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve the submitted expense reports for Project X."

**🤖 AI Agent:**
> There are 4 active expense reports for Project X totaling $1,250.30.

---

**👤 You:**
> "List all pending timesheets for the engineering department this week."

**🤖 AI Agent:**
> Querying Unanet timesheets ('get_timesheets')...
Found 3 pending timesheets for Engineering (Oct 18-24):
1. Alice Baker: 38 hrs (Awaiting Mgr Approval)
2. Charlie P.: 40 hrs (Draft)
3. Dave R.: 32 hrs (Draft)

---

**👤 You:**
> "Check the current compliance status and budget utilization for the 'Alpha-1' defense contract."

**🤖 AI Agent:**
> Analyzing project records ('get_project_details')...
Contract 'Alpha-1' (ID: DEF-771):
- Compliance: DCAA compliant tracking active, 100% compliant.
- Budget: $250,000
- Utilized: $145,200 (58%)
- Status: On Track.


## Installation & Usage

To install and use the **Unanet** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unanet](https://vinkius.com/mcp/unanet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
