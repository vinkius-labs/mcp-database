# Beagle Security MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/beagle-security-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Scan your web applications for vulnerabilities, generate penetration test reports, and strengthen your security posture proactively.

## Description
Connect your **Beagle Security** account to any AI agent and take full control of your automated cybersecurity audits and web application penetration testing through natural conversation.

### What you can do

- **Pentest Orchestration** — Programmatically trigger high-fidelity penetration tests for your configured web applications and APIs directly through your agent
- **Real-Time Monitoring** — Monitor the progress and status of active security tests and retrieve real-time alerts for identified threats
- **Vulnerability Intelligence** — Access complete high-fidelity vulnerability reports in JSON format and retrieve detailed metadata for every security session
- **Application Architecture** — List and manage your directory of security projects and applications to maintain a perfectly coordinated audit infrastructure
- **Audit Compliance** — Access historical records of all past test results and monitor currently running tests to ensure constant security oversight

### How it works

1. Subscribe to this server
2. Retrieve your **Access Token** (User Settings) and **Application Token** (Project Settings) from the Beagle Security dashboard
3. Start orchestrating your cybersecurity defenses from Claude, Cursor, or any MCP client

No more manual toggling between security scanners or digging through fragmented audit reports. Your AI acts as your dedicated security engineer and penetration testing coordinator.

### Who is this for?

- **Security Engineers** — instantly trigger regression tests and analyze vulnerability patterns using natural language commands
- **DevOps Teams** — verify application security after a deployment and monitor API health without leaving your workspace
- **CISOs & IT Leads** — automate the oversight of organization-wide security posture through simple AI queries


## Available Tools
- **get_application**: Get details of the current application
- **get_running_tests**: List all currently running tests
- **get_test_result**: Get full test result (JSON)
- **get_test_sessions**: List all test sessions
- **get_test_status**: Get current test status
- **list_applications**: List all applications
- **list_projects**: List all security projects
- **start_test**: Start a new security test
- **stop_test**: Stop a running security test


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Beagle Security** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all security applications configured in my Beagle account."

**🤖 AI Agent:**
> I've retrieved your application directory. You currently have 3 configured endpoints, including 'Main Website' and 'API v1'. Would you like to check the last test session for any of them?

---

**👤 You:**
> "Start a new penetration test for the current application."

**🤖 AI Agent:**
> Security audit triggered! I've initiated a new high-fidelity penetration test for your application. The test is now running in the cloud. I'll monitor the progress and notify you of any critical threats.

---

**👤 You:**
> "What is the status of the current security test?"

**🤖 AI Agent:**
> Fetching status... The current test is 'In Progress' (45% complete). So far, I've identified 2 low-risk items and 0 critical vulnerabilities. Shall I retrieve the real-time activity logs?


## ❓ FAQ

**Q: How do I find my Beagle Access and Application Tokens?**
Log in to Beagle Security. find the Access Token in your profile/user settings, and the Application Token in the settings of the specific project you want to test.

**Q: Can I stop a running test via AI?**
Yes! The `stop_test` tool allows your agent to immediately terminate an active penetration test for the configured application.

**Q: How do I retrieve the vulnerability report?**
First use `get_test_sessions` to identify the test's `resultToken`, then pass that token to `get_test_result` to retrieve the high-fidelity JSON report.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/beagle-security-alternative](https://vinkius.com/mcp/beagle-security-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Beagle Security** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `beagle-security-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Beagle Security** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "beagle-security-alternative": {
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
