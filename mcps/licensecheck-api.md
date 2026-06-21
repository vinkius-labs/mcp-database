# LicenseCheck API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/licensecheck-api)
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


## Available Tools (4)
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


## ❓ FAQ

**Q: How do I find my LicenseCheck API Key?**
Log in to your [**LicenseCheck account**](https://licenseapi.dev/), and you will find your API Key in your dashboard or profile settings. Copy and paste it below.

**Q: What types of licenses are covered?**
The API covers thousands of common open-source licenses (like MIT, Apache, GPL) as well as various proprietary and commercial licensing models.

**Q: Can the agent check for specific permissions?**
Yes. Every license record retrieved by your agent includes metadata on permitted actions, such as commercial use, distribution, and modification.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/licensecheck-api](https://vinkius.com/mcp/licensecheck-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LicenseCheck API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `licensecheck-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LicenseCheck API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "licensecheck-api": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
