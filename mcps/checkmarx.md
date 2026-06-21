# Checkmarx MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/checkmarx)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Automate AppSec via Checkmarx One — trigger core scans, analyze vulnerabilities, discover Best Fix Locations (BFL), and monitor KICS results.

## Description
Connect your **Checkmarx One** enterprise environment to any AI agent and take programmatic control over your Application Security posture. Analyze deep code flaws through natural chat instead of navigating complex cyber dashboards.

### What you can do

- **Projects & Applications** — Inventory your codebase containers, inspect active project linkages, and prepare specific branches for security scanning
- **Scans Lifecycle** — Trigger dynamic SAST/SCA security scans on repos, cancel redundant queues, and poll engines for precise execution timing
- **Vulnerability Triage** — Extract core datasets of severe vulnerabilities, mapping exact lines of code where the flawed logic resides
- **Best Fix Location (BFL)** — Ask the agent to calculate the exact optimal spot in your execution path to apply a patch that resolves the flaw entirely
- **KICS (IaC)** — Read specialized Infrastructure as Code metrics isolating misconfigurations exclusively in Terraform, Dockerfiles, or Kubernetes YAML

### How it works

1. Subscribe to this server
2. Provide your Checkmarx One JWT Token
3. Uncover code vulnerabilities natively inside Claude, Cursor, or any compatible MCP agent

### Who is this for?

- **Security Engineers (AppSec)** — seamlessly orchestrate vulnerability triage without toggling away from your primary workstation or ticket tracker
- **DevOps & Platform Teams** — investigate misconfigured KICS results in staging branches actively through the agent before deploying
- **Developers** — grab the exact Best Fix Location (BFL) for a zero-day issue and ask the LLM to rewrite the sanitization logic instantly


## Available Tools
- **cancel_scan**: Prevents unnecessary engine resource consumption and drops the scanning context if the developer pushed a new commit overlapping the running job.

Cancel an actively running Checkmarx scan
- **get_project**: Essential for ensuring the correct branch and source control context is selected before triggering new scans.

Get details for a specific Checkmarx project
- **get_kics_results**: Focuses solely on Terraform, CloudFormation, Kubernetes YAML, and Dockerfile misconfigurations rather than typical application source code flaws.

Get specialized Infrastructure as Code (KICS) findings
- **list_applications**: An Application acts as an overarching container for multiple individual microservices or projects, providing aggregated risk reporting and security metric visibility across a logical product.

List Checkmarx One Applications
- **list_bfl**: Provide the scan ID and the specific query (rule) ID string.

Get Best Fix Location (BFL) for a specific vulnerability node
- **list_projects**: A Project represents a specific codebase. Includes project metadata, IDs, and assigned application linkages.

List all Checkmarx One Projects
- **list_scans**: Includes the scan ID, current status (Completed, Running, Failed, Canceled), branch targeted, and timestamps. Use the scan ID to fetch the actual vulnerability results.

List all historical and active scans for a Checkmarx project
- **run_scan**: Extensively used in CI/CD integrations to assert security quality on PRs. Returns the ID of the newly queued scan.

Trigger a new Checkmarx One code scan
- **get_scan_details**: It returns granular execution details including which scan engines (SAST, SCA, KICS) were fired, their individual execution timings, and any engine-specific failure reasons.

Check the precise status and configuration of a Checkmarx scan
- **get_scan_results**: Each result includes the vulnerability severity, state (To Verify, Confirmed, Urgent), description, and the exact lines of code where the flaw was detected. Requires a completed scan ID.

Download SAST and security vulnerability findings for a scan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Checkmarx** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most severe vulnerabilities found in the last Checkmarx scan."

**🤖 AI Agent:**
> Found 12 vulnerabilities in scan #4521. Critical: 2 SQL Injection (CWE-89) in `/api/users.js:142` and `/auth/login.ts:87`. High: 3 XSS (CWE-79). Medium: 7. Use `get_bfl` to find the optimal fix location for each.

---

**👤 You:**
> "Trigger a new SAST scan for my current Checkmarx project."

**🤖 AI Agent:**
> SAST scan initiated successfully for project 'web-app' on branch 'main'. Scan ID: #4522. Estimated completion: ~8 minutes. I'll notify you when results are ready.

---

**👤 You:**
> "How do I fix the SQL injection vulnerability found in the Checkmarx report?"

**🤖 AI Agent:**
> The SQL injection in `auth/login.ts:87` can be fixed by using parameterized queries. Best Fix Location (BFL) analysis shows the root cause is at line 82 where user input flows unsanitized into the query builder. Replace the string concatenation with a prepared statement.


## ❓ FAQ

**Q: How can the AI help me fix a vulnerability faster?**
Once an issue is identified via scan results, ask your agent to pull the 'Best Fix Location' (BFL) using the query ID. Checkmarx mathematically finds the common root code block, and your AI can instantly rewrite that exact block to sanitize the flaw. You save hours tracing code paths.

**Q: Can the agent initiate a static code scan independently?**
Yes! Tell the agent to 'Run a scan on project ID X targeting the main branch'. It initiates the analysis array natively across Checkmarx One engines. You can poll for completion status later and retrieve the new dataset directly via chat.

**Q: Does it segregate AppSec results from Cloud infrastructure flaws?**
It does. Application flaws are pulled cleanly via `get_scan_results`, whereas misconfigurations tied to Docker, Kubernetes, or Terraform limits use a dedicated `get_kics_results` pipeline. The agent intrinsically separates the context for your DevOps team.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/checkmarx](https://vinkius.com/mcp/checkmarx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Checkmarx** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `checkmarx` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Checkmarx** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "checkmarx": {
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
