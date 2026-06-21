# SonarQube & SonarCloud MCP Server

Bring your standalone or cloud SonarQube quality gates native to your AI logic. Find bugs, duplications, and rewrite vulnerable code instantly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sonarqube-sonarcloud)

## Overview
**Category:** ship-it
**Tools Count:** 10

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


## Installation & Usage

To install and use the **SonarQube & SonarCloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sonarqube-sonarcloud](https://vinkius.com/mcp/sonarqube-sonarcloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
