# LicenseCheck API MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/licensecheck-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/licensecheck-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/licensecheck-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Search software licenses — audit permissions and conditions via AI.

## Description
Empower your AI agent to orchestrate your entire software compliance and license auditing workflow with **LicenseCheck**, the specialized source for open-source and proprietary license data. By connecting the LicenseAPI.dev service to your agent, you transform complex legal lookups into a natural conversation. Your agent can instantly retrieve license details, audit permissions and conditions, and query limitations without you ever touching a legal portal. Whether you are conducting dependency research or managing corporate compliance, your agent acts as a real-time legal consultant, ensuring your licensing data is always verified and precise.

### What you can do

- **License Auditing** — Search for thousands of software licenses by name or ID and retrieve detailed metadata, including versions and IDs.
- **Permission Oversight** — Audit specific permissions allowed by a license to understand the legal reach of your software usage instantly.
- **Condition Discovery** — Query mandatory conditions required by specific licenses to assist in compliance and archival planning.
- **Legal Intelligence** — Retrieve limitations and prohibitions for any license to identify relevant risk markers for your project.
- **Compliance Monitoring** — Check API status to ensure your legal research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your LicenseCheck API Key
3. Start managing your compliance intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal Tech & Compliance Officers** — monitor license terms and retrieve official metadata straight from your workflow.
- **Software Architects** — verify license compatibility and audit dependency patterns without manual searching.
- **Open Source Maintainers** — perform rapid audits of license requirements and identify relevant legal markers through natural language.
- **Operations Leads** — automate legal data querying to orchestrate cross-functional development teams smoothly.


## Available Tools
- **check_software_license**: Search for a software license by name or identifier
- **check_api_status**: dev REST API.

Check if the LicenseCheck service is operational
- **get_license_details**: Get full details and legal metadata for a specific license by ID
- **list_all_licenses**: List all software licenses available in the database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LicenseCheck API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the software license 'MIT' using LicenseCheck."

**🤖 AI Agent:**
> I've retrieved the details for the MIT license! It is a short and permissive license that allows for commercial use, distribution, and modification. Notable conditions include including the copyright notice. Would you like the full legal metadata?

---

**👤 You:**
> "What are the limitations of the 'GPL-3.0' license?"

**🤖 AI Agent:**
> I've identified the limitations for GPL-3.0. It is a copyleft license that requires derivatives to be licensed under the same terms. Notable limitations include liability and warranty disclaimers. I can provide the full list of conditions if you'd like.

---

**👤 You:**
> "List all software licenses available in the database."

**🤖 AI Agent:**
> I've scanned the license catalog from LicenseCheck! There are hundreds of licenses listed, from common open-source ones to specialized proprietary models. I can assist you with a keyword search to identify the exact markers for your audit.


## Installation & Usage

To install and use the **LicenseCheck API** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/licensecheck-api](https://vinkius.com/mcp/licensecheck-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
