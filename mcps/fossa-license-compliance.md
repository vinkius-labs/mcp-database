# FOSSA (License Compliance) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fossa-license-compliance)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage license compliance and security vulnerabilities via FOSSA — list projects, inspect revisions, and track dependencies directly from your AI agent.

## Description
Connect your **FOSSA** account to any AI agent to automate open-source license compliance and security auditing through natural language.

### What you can do

- **Project Overview** — List all projects in your organization with support for filtering and pagination.
- **Revision Tracking** — Access specific project revisions and fetch detailed metadata for any version locator.
- **Dependency Analysis** — Deep-dive into the dependency tree of any revision to understand your software bill of materials (SBOM).
- **Impact Assessment** — Identify every parent project that contains a specific vulnerable or non-compliant dependency.
- **Vulnerability Scanning** — Check for security vulnerabilities across multiple dependency locators in a single query.

### How it works

1. Subscribe to this server
2. Enter your FOSSA API Token
3. Start auditing your software supply chain from Claude, Cursor, or any MCP client

### Who is this for?

- **Security Engineers** — quickly identify where vulnerable packages are used across the entire organization.
- **Legal & Compliance Teams** — audit project revisions for license compliance without manually navigating the FOSSA UI.
- **DevOps & Architects** — verify dependency trees and project metadata directly from the terminal or code editor.


## Available Tools (6)
- **list_projects**: Supports filtering and pagination.

List all projects in your organization
- **get_revision_dependencies**: Get dependencies for a specific revision
- **list_revisions**: List revisions of a project
- **check_vulnerabilities**: Uses a POST request but only reads data.

Check vulnerabilities by dependency locators
- **get_revision**: Get details for a specific revision
- **get_parent_projects**: Get parent projects containing a dependency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FOSSA (License Compliance)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all projects in my FOSSA organization named 'DocsExample'."

**🤖 AI Agent:**
> I've found the project: 'custom+27932/DocsExample'. Would you like to see its recent revisions or check for vulnerabilities?

---

**👤 You:**
> "Check for vulnerabilities in npm+ssh2$0.6.1 and npm+coa$2.0.2."

**🤖 AI Agent:**
> I've analyzed those locators. 'npm+ssh2$0.6.1' has 2 critical vulnerabilities related to command injection. 'npm+coa$2.0.2' is currently clear of known vulnerabilities in the FOSSA database.

---

**👤 You:**
> "Which projects are using the dependency npm+coa$2.0.2?"

**🤖 AI Agent:**
> The dependency 'npm+coa$2.0.2' is found in 3 parent projects: 'Core-API', 'Frontend-Dashboard', and 'Legacy-Auth-Service'.


## ❓ FAQ

**Q: Can I find which projects are affected by a specific vulnerable package?**
Yes. Use the `get_parent_projects` tool with the dependency locator (e.g., `npm+coa$2.0.2`) to see every project in your organization that includes that specific dependency.

**Q: How do I check for security vulnerabilities in a list of dependencies?**
You can use the `check_vulnerabilities` tool by providing an array of dependency locators. The agent will return any known security issues impacting those specific versions.

**Q: Can I see the full dependency list for a specific project version?**
Absolutely. By using `get_revision_dependencies` with a revision locator, you can retrieve the complete list of dependencies identified by FOSSA for that specific build or release.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fossa-license-compliance](https://vinkius.com/mcp/fossa-license-compliance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FOSSA (License Compliance)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fossa-license-compliance` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FOSSA (License Compliance)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fossa-license-compliance": {
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
