# SonarCloud MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sonarcloud)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sonarcloud-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sonarcloud-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Merge your SaaS DevOps workflow with SonarCloud to review AI code and prevent production vulnerabilities.

## Description
Bring **SonarCloud’s** industry-leading static code analysis and quality gate checks natively to your AI assistant. Eliminate manual portal checks by querying project bugs, technical debt metrics, and security hotspots dynamically inside your editor via the MCP protocol. Ensure the AI writes secure, compliant data structures aligned with your strict SonarCloud CI/CD definitions.

### What you can do

- **Project Surveillance** — Discover application projects via `search_projects` and fetch internal component hierarchies calling `list_project_components`
- **Vulnerability Hunting** — Expose specific codebase flaws instantly with `search_issues`, extracting actionable remediation steps querying `get_issue_details`
- **Quality Check** — Inspect code passing grades via `get_quality_gate_status` and retrieve specific KPI metrics like coverage using `get_project_measures`
- **Operation Controls** — Pull your organizations (`list_organizations`) and team members (`search_users`) actively tied to specific code repositories

### How it works

1. Subscribe to this AI integration server
2. Introduce your personal SonarCloud Security Token
3. Instruct your local AI assistant to verify project coverage before pushing a PR

Stop digging through the SonarCloud UI just to see why an automated test or quality gate failed. Find the precise faulty dependency versions instantly within your codebase context.

### Who is this for?

- **Software Developers** — request a quick scan check over your latest component before a CI/CD build starts complaining
- **DevSecOps** — query exact details on failing quality gates prior to approving PR merges
- **Team Leads** — gather accurate metrics like lines of code or code coverage directly via textual prompts without opening analytical dashboards


## Available Tools
- **get_issue_details**: Retrieves details for a specific issue
- **get_project_measures**: Requires project key and comma-separated metric keys.

Retrieves quality measures for a specific project component
- **get_analysis_status**: Retrieves the latest analysis status for a project
- **get_quality_gate_status**: g., "OK", "ERROR").

Retrieves the quality gate status for a project
- **list_project_components**: Lists files and directories (components) within a project
- **list_organizations**: Lists organizations for the current user
- **search_issues**: Filter by component (project) key.

Searches for code quality issues
- **search_projects**: You can filter by organization key.

Searches for projects in SonarCloud
- **search_users**: Searches for users in the organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SonarCloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the quality gate status of the main monolith backend project in SonarCloud."

**🤖 AI Agent:**
> Querying `get_quality_gate_status` for `monolito-backend-core`:
**Status: ERROR 🔴**

The Quality Gate failed because new code coverage dropped natively to 74% (against the 80% mandatory target) and 2 new code smells were introduced. Want me to dive deeper into `search_issues` to list the bad smells?

---

**👤 You:**
> "List all registered organizations tied to my SonarCloud profile along with our connected users."

**🤖 AI Agent:**
> Running organizational discovery (`list_organizations`) and user lookup (`search_users`).

**Organizations**:
- 🏢 `vinkius-global-labs` (Name: VinkiusLabs LLC)
- 🏢 `personal-dev-sandbox` (Name: Renan Sandbox Hub)

**Active Users under Global Scope**:
- `renato_admin` (Active)
- `carlos_dev` (Active)
- `samuel_ci_bot` (Service Account)

Let me know if you need specific details for one logical group alone.

---

**👤 You:**
> "Pull all the 'Major' and 'Critical' open issues for the API backend service codebase."

**🤖 AI Agent:**
> Accessing `search_issues` filtering dynamically for CRITICAL and MAJOR severities assigned to target `api-backend-srv`.

**Detected Issues (Filtered View):**
1. 🚨 **CRITICAL** (Bug): `NullPointerException` likely in `src/auth/tokenValidator.js` line 44 (Key: `AXb13k`)
2. 🚨 **CRITICAL** (Vulnerability): Hardcoded token visible in class `EmailMailer` at `src/services/mail.js` (Key: `AWz1L2`)
3. ⚠️ **MAJOR** (Code Smell): Cognitive complexity of `handleUserProcess()` exceeds tier 18 inside `controller.js` (Key: `AYx99m`)


## Installation & Usage

To install and use the **SonarCloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sonarcloud](https://vinkius.com/mcp/sonarcloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
