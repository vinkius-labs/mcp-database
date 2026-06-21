# Semgrep MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/semgrep)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Equip your AI agent with read/write access to Semgrep's SAST platform to audit code security findings, update triage statuses, and enforce custom semantic rules.

## Description
Connect the **Semgrep** AppSec platform directly to your AI agent to radically accelerate code security triaging. Instead of forcing developers to jump between their IDE and the Semgrep dashboard, empower your AI to pull 'Findings', analyze the vulnerable syntax, and instantly close false positives.

### What you can do

- **Triage Findings (Bugs)** — Instruct the agent to grab the latest CI vulnerability findings and immediately push a status update to mark it as fixed, ignored, or mitigated (`update_finding_status`)
- **Rule Management** — Request the AI to look at a newly discovered bad coding pattern and command it to write and deploy a matching custom semantic rule (`create_rule`) to your organizational deployment
- **Project & Deployment Scoping** — Map out all repositories running Semgrep actions and check their overarching security health scores in milliseconds
- **Comprehensive Forensics** — Fetch granular SCA and SAST semantic flaw definitions, including exact snippets, CVE links, and the specific bad lines causing the trigger

### How it works

1. Enable this MCP server within your workflow
2. Supply a standard API Token from your Semgrep Dashboard settings
3. Engage your agent in Cursor or Claude to cross-examine security warnings dynamically

### Who is this for?

- **Security Engineers (AppSec)** — tell the AI to quickly delete an obsolete rule across the entire deployment without wrestling with the dashboard interface
- **DevOps** — retrieve compliance metrics and pipeline fix rates natively and pipe them directly into an executive summary report via chat
- **Software Developers** — let Cursor fetch the specific `finding_id` blocking your PR, explain what the vulnerability means, and draft the exact semantic fix to pass the scan


## Available Tools
- **create_rule**: Allows developers to forbid project-specific bad patterns securely and continuously across the enterprise repositories.

Create a customized Semgrep security rule within the platform
- **delete_rule**: Delete a custom Semgrep security rule from the deployment
- **list_deployments**: The primary key is the deployment slug identifier. Almost all subsequent API operations targeting rules, projects, or findings will require this deployment slug to define the scope.

List Semgrep organizational deployments
- **list_findings**: Findings provide snippet details, file line numbers, severity, and rule types.

Fetch global static analysis security findings for a deployment
- **get_finding_details**: Explains the exact malicious code block, suggests semantic fixes, states whether it is blocking PRs in CI, and links to CVE data (if an SCA supply chain defect).

Get atomic details for a specific Semgrep flaw
- **get_project**: Search for a precise Semgrep project by exact repository name
- **list_rules**: The rules are structured YAML definitions that search for semantic anti-patterns in codebases (e.g., unparameterized SQL queries, hardcoded AWS keys).

List Semgrep semantic rules deployed globally
- **get_metrics**: Typically consumed to render executive security dashboards.

Get AppSec metrics and compliance stats for Semgrep
- **list_projects**: Projects maintain a link between developers and static security scan outputs over time.

List Semgrep projects (repositories) monitored in a deployment
- **update_finding_status**: Valid states generally include active, fixed, false_positive, ignored, mitigated. Resolving findings through this API cleans up the developer experience when managing compliance queues.

Mark a Semgrep finding state (e.g., fixed, false positive)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Semgrep** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most severe unmitigated findings currently breaking our CI/CD pipeline on the 'vinkius/cloud' repository."

**🤖 AI Agent:**
> I've fetched the findings list scoped to 'vinkius/cloud'. Currently, there are 2 blockers. 1) Exposed hardcoded AWS Secret Access Key in `auth.py:L45`. 2) Outdated dependency `lodash@4.17.15` in `package.json` vulnerable to prototype pollution. Would you like me to resolve the Lodash one by generating an update commit script?

---

**👤 You:**
> "Mark vulnerability issue ID #58032 as a 'false_positive' using the update finding tool."

**🤖 AI Agent:**
> The operation is complete. I've sent the mutation `update_finding_status` for issue 58032 within your deployment. Semgrep now permanently recognizes this event as `false_positive`, and subsequent scans will not flag this specific semantic line match again.

---

**👤 You:**
> "Review the company's Semgrep performance metrics focusing on fix rate."

**🤖 AI Agent:**
> I've analyzed your AppSec timeline with `get_metrics`. Your overall Fix Rate for the trailing 30 days is hovering around 83%. The median 'time-to-resolve' for critical SAST vulnerabilities is 3.4 days. This shows strong engagement natively within developer pull requests before merge.


## ❓ FAQ

**Q: Can the AI resolve or close findings in Semgrep natively?**
Yes. This server supports mutable actions. By invoking `update_finding_status`, your AI agent can shift a specific semantic flaw to 'mitigated', 'fixed', 'ignored', or 'false_positive' updating the registry in real-time.

**Q: How can I deploy a new custom SAST rule via chat?**
Simply ask the LLM: 'Draft a semantic grep rule to ban hardcoded API keys in Python and deploy it'. The agent will natively format the JSON structure required and call `create_rule`, sending it directly to all repositories.

**Q: Do I need to supply a 'Deployment Slug' for every request?**
Most API queries require the deployment context. To ensure smooth interactions, just tell the agent your organization slug once (or let it query `list_deployments` to fetch the default one). The agent will remember it for the rest of the conversation loop.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/semgrep](https://vinkius.com/mcp/semgrep)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Semgrep** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `semgrep` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Semgrep** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "semgrep": {
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
