# DeepSource MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deepsource)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate code quality monitoring via DeepSource — analyze issues, vulnerabilities, metrics, and report cards directly from any AI agent.

## Description
Connect your **DeepSource** account to any AI agent and take full control of code quality analysis, vulnerability detection, and metrics monitoring through natural conversation.

### What you can do

- **Code Issues** — List and inspect code quality issues (code smells, anti-patterns, bugs) across repositories with severity and file locations
- **Analysis History** — View recent analysis runs with status, branch, and analyzer information (Python, JavaScript, Go, etc.)
- **Security Vulnerabilities** — Identify dependency vulnerabilities (SCA) with CVE IDs, CVSS scores, reachability, and fixability status
- **Code Metrics** — Query maintainability index, cyclomatic complexity, lines of code, and test coverage percentages
- **Report Cards** — Get overall repository health grades (A-F) with score breakdowns and trend analysis
- **SCA Targets** — List all dependency manifest files being scanned for supply chain security
- **Repository Management** — Activate/deactivate repos, update default branches, and regenerate DSN tokens

### How it works

1. Subscribe to this server
2. Enter your DeepSource Personal Access Token
3. Start monitoring code quality, reviewing issues, and tracking vulnerabilities from Claude, Cursor, or any MCP-compatible client

No more manual navigation through the DeepSource dashboard. Your AI acts as a dedicated code quality analyst or security reviewer.

### Who is this for?

- **Engineering Managers** — instantly review code quality grades, issue counts, and analysis status across multiple repositories without opening the dashboard
- **Security Teams** — monitor dependency vulnerabilities with CVE details, CVSS scores, and prioritize remediation based on reachability
- **Developers** — check code issues, metrics, and report cards directly from the IDE to fix quality problems before merging
- **DevOps Leads** — manage repository activation status, default branches, and DSN rotation across the organization


## Available Tools (14)
- **update_default_branch**: This affects which branch is analyzed by default.
You must provide the repository ID (from get_repository) and the new branch name (e.g., "main", "develop", "master").
Use this when your team changes the default branch name (e.g., migrating from "master" to "main").

Update the default branch for a repository in DeepSource
- **activate_repository**: Once activated, DeepSource will start analyzing the code on each push/PR.
You must provide the repository ID (obtained from get_repository).
Use this to enable code quality monitoring for a repository that was previously inactive.

Activate a repository for code analysis in DeepSource
- **deactivate_repository**: No new analyses will run until the repository is reactivated.
You must provide the repository ID (obtained from get_repository).
Use this to pause analysis for archived repositories or when you want to stop billing for a specific repository.

Deactivate a repository to stop code analysis in DeepSource
- **get_report_card**: This provides a quick health check of the repository's overall code quality status.
You must provide the repository name, login, and VCS provider.
Use this to get a high-level view of code quality trends and identify areas needing improvement.

Get the overall report card (grade) for a repository
- **get_repository_metrics**: You must provide the repository name, login, and VCS provider.
Optionally filter by specific metric shortcodes (e.g., "LCV" for line coverage, "MI" for maintainability index, "CC" for cyclomatic complexity).
If no shortcodes specified, returns all available metrics with their values and thresholds.

Get code quality metrics for a repository
- **get_repository**: You must provide the repository name, login (user or org name), and VCS provider (e.g., GITHUB, GITLAB, BITBUCKET).
Use this to inspect repository configuration before querying issues, analyses, or metrics.

Get details of a specific repository in DeepSource
- **get_test_coverage**: Shows the coverage percentage value and any configured thresholds.
You must provide the repository name, login, and VCS provider.
Use this to monitor code quality and ensure adequate test coverage across your codebase.

Get test coverage metrics for a repository
- **get_viewer**: Use this to verify your API token is working and to get your user details from DeepSource.

Get the authenticated user profile from DeepSource
- **get_vulnerability**: You must provide the repository name, login, VCS provider, and the vulnerability occurrence ID (obtained from list_vulnerabilities).
Use this to deep-dive into a specific vulnerability before deciding on remediation steps.

Get details of a specific dependency vulnerability by its ID
- **list_analysis_runs**: You must provide the repository name, login, and VCS provider.
Optionally filter by branch name and limit the number of results (default: 20).
Each run shows which analyzer was used (e.g., PYTHON, JAVASCRIPT, GO) and whether the analysis succeeded or failed.

List recent code analysis runs for a repository
- **list_issues**: You must provide the repository name, login, and VCS provider.
Optionally filter by analyzer short code (e.g., "PYTHON", "JS-A1") and limit results (default: 50).
Each issue includes up to 3 sample occurrences with file path and line number.
Use this to identify code smells, anti-patterns, and potential bugs across your codebase.

List code quality issues in a repository
- **list_sca_targets**: Each target includes ecosystem (e.g., npm, pip, gem), package manager, manifest file path, and activation status.
You must provide the repository name, login, and VCS provider.
Use this to understand which dependency files are being scanned for vulnerabilities.

List all SCA (Supply Chain Analysis) targets in a repository
- **list_vulnerabilities**: Each vulnerability includes severity, CVE ID, CVSS score, description, affected package name and version, reachability status, and fixability.
You must provide the repository name, login, and VCS provider.
Optionally limit the number of results (default: 20).
Use this to identify security risks in your dependencies and prioritize remediation.

List dependency vulnerabilities in a repository (SCA)
- **regenerate_dsn**: The DSN is used to authenticate DeepSource analysis runs.
You must provide the repository ID (obtained from get_repository).
This action invalidates the old DSN and returns the new one. Use this if you suspect the DSN has been compromised or needs rotation.

Regenerate the DSN (Data Source Name) for a repository


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DeepSource** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the overall code quality report card and current issues for the 'api-service' repository in the 'acme-corp' GitHub organization."

**🤖 AI Agent:**
> I've retrieved the report card for 'api-service'. Current Grade: **B+** (Score: 87/100). Issues Summary: 12 total (3 CRITICAL, 4 HIGH, 5 MEDIUM). Most critical issues include: unused imports (PYTHON-E1203) in 4 files, potential SQL injection risk (PYTHON-S5001) in auth module, and high cyclomatic complexity (CC>10) in 2 functions. Last analysis: 2 hours ago on branch 'main'. Would you like the full details of any specific issue?

---

**👤 You:**
> "Check for any critical or high severity dependency vulnerabilities in the 'web-frontend' repo and tell me which packages are affected."

**🤖 AI Agent:**
> I found 5 dependency vulnerabilities in 'web-frontend':

1. **CVE-2024-1234** (CRITICAL, CVSS: 9.8) — `lodash@4.17.20` — Prototype Pollution. Fix available in v4.17.21. Reachable: Yes.
2. **CVE-2024-5678** (HIGH, CVSS: 7.5) — `express@4.17.1` — Open Redirect vulnerability. Fix available in v4.18.0. Reachable: Yes.
3. **CVE-2023-9012** (HIGH, CVSS: 7.2) — `axios@0.21.1` — SSRF vulnerability. Fix available in v1.6.0. Reachable: No.
4. **CVE-2024-3456** (MEDIUM, CVSS: 5.3) — `minimist@1.2.5` — Prototype Pollution. Fix available in v1.2.6.
5. **CVE-2023-7890** (MEDIUM, CVSS: 4.9) — `node-fetch@2.6.1` — Information Exposure. Fix available in v3.0.0.

Recommended action: Upgrade lodash and express immediately due to high reachability and severity.

---

**👤 You:**
> "What's the test coverage for our 'backend-api' repository and show me the most recent analysis runs?"

**🤖 AI Agent:**
> I've retrieved the data for 'backend-api':

**Test Coverage**: 78.5% (Line Coverage - LCV). Threshold configured: 80%. You're slightly below target.

**Recent Analysis Runs** (last 5):
1. Run #abc123 — Status: PASSED — Branch: main — Analyzer: PYTHON — 2 hours ago
2. Run #def456 — Status: PASSED — Branch: feature/auth — Analyzer: PYTHON — 5 hours ago
3. Run #ghi789 — Status: FAILED — Branch: feature/payments — Analyzer: PYTHON — Yesterday — Error: timeout
4. Run #jkl012 — Status: PASSED — Branch: main — Analyzer: JS-A1 — Yesterday
5. Run #mno345 — Status: PASSED — Branch: develop — Analyzer: PYTHON — 2 days ago

Would you like to see what issues were found in the most recent run, or should I help investigate the failed payment analysis?


## ❓ FAQ

**Q: How do I get a DeepSource Personal Access Token and where do I find it?**
Log in to your DeepSource account, go to **Account Settings** → **Personal Access Tokens**, and click **Create New Token**. Give it a descriptive name (e.g., 'Vinkius MCP') and copy the token immediately — it won't be shown again. Paste this token into the API key field below. The token is used as a Bearer token in the Authorization header for all GraphQL requests to `https://api.deepsource.com/graphql/`.

**Q: What types of code issues can DeepSource detect and how are they categorized?**
DeepSource detects various code quality issues including code smells, anti-patterns, performance issues, security vulnerabilities, and bugs. Issues are categorized by severity (CRITICAL, HIGH, MEDIUM, LOW) and by analyzer type (e.g., PYTHON for Python issues, JS-A1 for JavaScript anti-patterns, GO for Go issues). Each issue includes a shortcode, title, category, and file locations with line numbers. You can filter issues by analyzer short code when querying repositories.

**Q: How does DeepSource detect dependency vulnerabilities and what information is provided?**
DeepSource uses Supply Chain Analysis (SCA) to scan dependency manifest files (package.json, requirements.txt, Gemfile, etc.) for known vulnerabilities. Each vulnerability includes: CVE ID, CVSS score (0-10), severity level, description, affected package name and version, ecosystem (npm, pip, etc.), reachability status (whether the vulnerable code is actually called), and fixability (whether a fix version is available). This helps prioritize which vulnerabilities to address first based on real risk rather than just theoretical severity.

**Q: What is the API rate limit and how many requests can I make per hour?**
DeepSource enforces a rate limit of 5,000 requests per hour per user account. This limit covers both read (queries) and write (mutations) operations. If you exceed this limit, the API will return HTTP 429 (Too Many Requests). For most code review and monitoring workflows, this limit is more than sufficient. If you need higher limits for large-scale analysis, contact DeepSource support.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deepsource](https://vinkius.com/mcp/deepsource)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DeepSource** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `deepsource` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DeepSource** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deepsource": {
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
