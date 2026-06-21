# 42Crunch MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/42crunch)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/42crunch-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/42crunch-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate API security testing via 42Crunch — manage collections, trigger audits, run conformance scans, and retrieve security reports directly from any AI agent.

## Description
Connect your **42Crunch** account to any AI agent to continuously test, audit, and secure your API lifecycle through natural conversation. Say goodbye to manual spec uploads and cumbersome dashboard navigations.

### What you can do

- **API Collections** — List and view your organizational API collections, evaluating their aggregated security scores
- **API Management** — Import OpenAPI/Swagger definitions directly into collections, list imported definitions, or delete them when decommissioned
- **Static Security Audits** — Trigger fresh static security audits over your OpenAPI specifications and retrieve comprehensive audit reports scoring design risks
- **Dynamic Conformance Scans** — List historical scans and retrieve detailed execution reports highlighting undocumented behavior or implementation flaws

### How it works

1. Subscribe to this server
2. Enter your 42Crunch API Token
3. Start managing your API security governance from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevSecOps Engineers** — integrate security audits seamlessly and ask for immediate remediation steps for OWASP vulnerabilities
- **Platform Teams** — govern your microservices ecosystem, track security hygiene across collections, and spot uncompliant endpoints
- **Backend Developers** — quickly import a new spec iteration, trigger a scan, and compare the security grade evolution without context switching


## Available Tools
- **get_audit_report**: Download the static security audit report for an API
- **delete_api**: Delete an API definition from the platform
- **get_api**: Get detailed metadata and score for a specific API
- **get_collection**: Get metadata and security score for a collection
- **import_api**: Import an OpenAPI definition into a collection
- **list_apis**: Each API entry includes its unique ID and security score.

List all API definitions within a collection
- **list_collections**: Use this to find the Collection ID you need to import or list APIs.

List all API collections in the platform
- **list_scans**: List dynamic conformance scans against a live API
- **get_scan_report**: Get detailed results from a dynamic conformance scan
- **trigger_audit**: Use this to trigger a scan after a specification gets updated.

Run a fresh static security audit on an API definition


## 💬 Prompt Examples

Here are some examples of how you can interact with the **42Crunch** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my API collections in 42Crunch."

**🤖 AI Agent:**
> You have 2 API collections:
1. Mobile Services (ID: c8b2f91a) - Score: 85/100, 4 APIs
2. Internal Microservices (ID: d9c3a10b) - Score: 62/100, 12 APIs
Would you like me to inspect the low-performing Internal Microservices collection?

---

**👤 You:**
> "Get the audit report for the 'User Management' API definition."

**🤖 AI Agent:**
> The 'User Management' API scored 55/100. Critical issues found:
- Missing rate limits on `/login` endpoint (CWE-307)
- OAuth2 configuration lacks detailed scope restrictions
- User schema accepts generic object data without type strictness
Should I propose the exact YAML additions required to resolve these?

---

**👤 You:**
> "Trigger a fresh security audit for API ID '2e4f0a91-db6c-4822-a9b0'."

**🤖 AI Agent:**
> A new static security audit has been triggered for the API definition. I will retrieve the fresh score and finding report momentarily...


## Installation & Usage

To install and use the **42Crunch** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/42crunch](https://vinkius.com/mcp/42crunch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
