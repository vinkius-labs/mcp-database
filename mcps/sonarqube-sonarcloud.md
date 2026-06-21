# SonarQube & SonarCloud MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sonarqube-sonarcloud)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sonarqube-sonarcloud-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sonarqube-sonarcloud-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Bring your standalone or cloud SonarQube quality gates native to your AI logic. Find bugs, duplications, and rewrite vulnerable code instantly.

## Description
Connect your self-hosted **SonarQube** instances or **SonarCloud** dashboards directly to your preferred AI agent. Speed up your DevSecOps workflow by diagnosing and investigating static code vulnerabilities via natural language. Rather than jumping between browser tabs trying to locate a specific Code Smell or Security Hotspot, query your organizational technical debt footprint dynamically through MCP.

### What you can do

- **Quality Gate Verification** — Stop bad commits before they happen. Ask your AI to `get_quality_gate_status` on your target project and pull KPIs like unit test coverage using `get_measures`
- **Vulnerability Hunting** — Expose specific codebase flaws instantly with `search_issues` filtering by severity (Critical, Blocker, Major)
- **Deep Code Insight** — Retrieve entire directories and component hierarchies calling `get_component_tree` and fetch raw annotated source code through `get_source_code`
- **Security & Rules** — Consult your enabled analysis rules directly via `list_rules` and audit manual-review `get_hotspots` on your main server

### How it works

1. Subscribe to this AI integration server
2. Introduce your Personal Target URL (e.g. `https://sonar.mycompany.intern` or `https://sonarcloud.io`)
3. Inject your Sonar User API Token securely
4. Start using Claude, Cursor, or your terminal IDE to command your static analysis

### Who is this for?

- **Software Engineers** — ask your local AI why Sonar blocked your PR merging process and demand an immediate, context-aware code refactor patch
- **DevSecOps** — query exact details on critical CVEs before approving PR merges, fetching raw SCM blame directly natively
- **Tech Leads** — gather project duplication ratios (`get_duplications`) or test coverage blindly mapping whole folders textually


## Available Tools
- **get_component_tree**: Get the component tree (files/directories) of a SonarQube project with metrics
- **get_duplications**: Get code duplication blocks for a file in SonarQube
- **get_hotspots**: Get security hotspots for a SonarQube project
- **get_measures**: Requires project key and comma-separated metric keys.

Get code quality measures/metrics for a SonarQube project
- **get_quality_gate_status**: Get the quality gate status for a SonarQube project
- **get_source_code**: Get annotated source code lines from SonarQube for a file
- **list_quality_gates**: List all quality gate definitions in SonarQube
- **list_rules**: Can filter by language.

List SonarQube analysis rules
- **search_issues**: Filter by project key and optional severities.

Search code issues in a SonarQube/SonarCloud project
- **search_projects**: Returns project keys and names. Project keys are required for most other tools.

Search projects on SonarQube/SonarCloud


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SonarQube & SonarCloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search our primary repository and give me the official Quality Gate diagnostic."

**🤖 AI Agent:**
> Running checks on `backend-main-api` using `get_quality_gate_status`.
**Gate Result: OK 🟢**

The most recent static checks successfully validated. Thresholds for Reliability facing bugs and Security ratings are comfortably within standard tolerance boundaries.

---

**👤 You:**
> "Run a test coverage and technical debt measure retrieval on all core services."

**🤖 AI Agent:**
> Invoked `get_measures` spanning metric keys `coverage,sqale_index` across your `core-srv-module` baseline.

- **Branch Coverage**: 85.3%
- **Line Coverage**: 81.6%
- **Tech Debt Rate**: 14h 22min (Sqale Index)

Do you want me to search issues to drop technical debt in half?

---

**👤 You:**
> "Tell me the precise component lines hitting security hotspot alerts."

**🤖 AI Agent:**
> Executing `get_hotspots` against origin `frontend-app-portal`:

1. 🔴 **Vulnerability Risk Level 1** -> Located in `pages/api/submit.js` (Component File)
- **Rule ID**: S1452 (Unvalidated Redirect / SSRF potential)
- **Line Source Area**: ~ L: 47

2. 🔴 **Vulnerability Risk Level 1** -> Located in `utils/hasher.js`
- **Rule ID**: S2278 (Weak cryptographic algorithm used for generic salts)

I can retrieve lines specifically natively via `get_source_code` if you're ready to fix this token loop now.


## Installation & Usage

To install and use the **SonarQube & SonarCloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sonarqube-sonarcloud](https://vinkius.com/mcp/sonarqube-sonarcloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
