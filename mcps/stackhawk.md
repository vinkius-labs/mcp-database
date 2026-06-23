# StackHawk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stackhawk)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Connect your AI to the StackHawk DAST platform. Run automated security scans, triage alerts seamlessly, and find vulnerabilities effortlessly.

## Description
Integrate the robust dynamic application security testing (DAST) capabilities of **StackHawk** directly into your conversational AI. Empower your engineering team to monitor system vulnerabilities, initiate complex scans, and orchestrate proactive security protocols without relying heavily on static dashboards. Connect securely to your workspaces, instruct your AI to assess ongoing security threats, and automatically classify alerts through a natural language interface designed to accelerate risk remediation across modern CI/CD pipelines.

### What you can do

- **Automated Scanning** — Programmatically initiate comprehensive security evaluations across your environments utilizing `run_scan`, and halt operations securely targeting specific execution UUIDs via `stop_scan`.
- **Risk Assessment** — Effectively audit environments by listing operational scans with `list_scans`, or retrieve deep vulnerability reports invoking `get_alerts` targeting specific scan iterations.
- **Application Management** — Catalog active software deployments monitored by StackHawk utilizing `list_applications`, and manage organizational parameters inspecting environments directly via `list_environments`.
- **Triage & Operations** — Authenticate securely establishing a valid operational bearer token with `login`, and instruct the AI to accurately qualify, dismiss, or assign statuses prioritizing critical mitigation efforts using `triage_alert`.

### How it works

1. Install the StackHawk MCP module configuring it directly with your active AI assistant.
2. Supply your proprietary StackHawk API Token to authenticate requests safely within the MCP setting.
3. Instruct the AI: "Retrieve the most critical security alerts from the last scan of our 'Production-Core' application, and triage any false positives."

### Who is this for?

- **DevSecOps Engineers** — Streamline and enforce secure software integration effortlessly instructing the system to perform real-time verification analysis dynamically.
- **Engineering Leaders** — Monitor organizational compliance metrics easily interacting through language commands retrieving holistic cross-application threat landscapes.
- **Backend Developers** — Quickly identify security regression issues caused by newly deployed microservices parsing scans directly in the development terminal.


## Available Tools (10)
- **get_application_details**: Get detailed configuration for a specific StackHawk application
- **get_organization_details**: Get StackHawk organization details and subscription tier
- **get_scan_alerts**: Download individual security alerts discovered by a DAST scan
- **get_scan_results**: Get detailed results and metadata for a specific DAST scan
- **list_applications**: Requires a Bearer token and organization ID.

List all registered DAST applications in a StackHawk organization
- **list_environments**: g., Development, Staging, Production) configured on the application.

List configured scan environments for a StackHawk application
- **list_api_keys**: Useful for auditing and hygiene.

List API keys configured for a StackHawk organization
- **list_scans**: Includes scan IDs and high-level alert counts.

List all DAST scan executions for a StackHawk application
- **login**: This token is required for all subsequent StackHawk tool calls.

Authenticate and obtain a Bearer access token from StackHawk
- **triage_alert**: Valid statuses: RISK_ACCEPTED, FALSE_POSITIVE, IN_PROGRESS.

Triage a DAST security alert (accept risk, false positive, etc.)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **StackHawk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Log in with my API token, list my projects and environments, then show the critical vulnerabilities from the latest scan."

**🤖 AI Agent:**
> Authentication successful. 🔒
**Applications (`list_applications`)**:
- `Payment-Gateway-Core`
- `Internal-Admin-Dashboard`

**Environments (`list_environments`)**:
- `Production`
- `Staging`

**Critical Alerts (`get_alerts`)**:
- SQL Injection — Risk: High — Endpoint: /api/auth

---

**👤 You:**
> "Run a new scan against the Production application."

**🤖 AI Agent:**
> Scan initiated via `run_scan`. ✅
The DAST audit is running asynchronously. Track progress with `list_scans` using the returned UUID.


## ❓ FAQ

**Q: Are scans executed locally or in the cloud?**
Scans run on the StackHawk cloud infrastructure. The MCP integration only triggers and monitors them — no heavy processing happens in your AI context.

**Q: Why is the `login` step required?**
The StackHawk API uses short-lived Bearer tokens. The `login` tool exchanges your API key for a session token that authenticates all subsequent requests.

**Q: Can the agent triage alerts automatically?**
Yes. Use `triage_alert` to mark specific vulnerabilities as false positives, accepted risks, or confirmed issues. Each triage action targets a single alert by ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stackhawk](https://vinkius.com/mcp/stackhawk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **StackHawk** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `stackhawk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **StackHawk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stackhawk": {
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
