# CI/CD Pipeline Config Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cicd-pipeline-config-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Deterministic validator for GitHub Actions and GitLab CI configuration files.

## Description
Ensure the structural integrity, security, and execution safety of your CI/CD pipelines. This MCP server provides specialized tools like `check_structure` to verify required keys, `validate_references` to enforce immutable SHA256 hashes for actions and images, and `audit_safety` to detect unbounded timeouts or missing error handling in shell scripts. Use `generate_compliance_report` for a comprehensive audit of your YAML configurations.


## Available Tools (4)
- **generate_compliance_report**: Generate a full compliance report for a pipeline
- **validate_references**: Validate that external references use immutable sha256 hashes
- **audit_safety**: Audit the pipeline for execution safety risks
- **check_structure**: Check the structural integrity of a CI/CD pipeline config


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CI/CD Pipeline Config Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is my GitHub Actions workflow structurally sound?"

**🤖 AI Agent:**
> The structural check for your configuration is complete. All required keys like 'on' and 'jobs' are present.

---

**👤 You:**
> "Check if my GitLab CI file has any security risks in its references."

**🤖 AI Agent:**
> The reference scan identified 1 invalid reference: 'docker.io/library/alpine:latest'. Please use a SHA256 hash instead.

---

**👤 You:**
> "Audit my pipeline for execution safety risks."

**🤖 AI Agent:**
> The audit found 1 violation: Unbounded timeout detected in job 'build'. Please specify 'timeout-minutes'.


## ❓ FAQ

**Q: What platforms are supported?**
The validator supports GITHUB_ACTIONS and GITLAB_CI configurations.

**Q: How does the tool ensure reference security?**
By using `validate_references`, the tool scans for any external references that do not use an immutable `@sha256:[hash]` format.

**Q: Can I get a full audit of my pipeline?**
Yes, the `generate_compliance_report` tool provides a consolidated report including syntax errors and best practice violations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cicd-pipeline-config-validator](https://vinkius.com/mcp/cicd-pipeline-config-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CI/CD Pipeline Config Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cicd-pipeline-config-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CI/CD Pipeline Config Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cicd-pipeline-config-validator": {
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
