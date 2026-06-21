# Epsilon3 Aerospace Operations MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/epsilon3-aerospace-operations)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/epsilon3-aerospace-operations-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/epsilon3-aerospace-operations-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Equip your AI agent to manage operational procedures, track execution runs, and monitor telemetry via the Epsilon3 API.

## Description
Integrate **Epsilon3**, the leading software platform for aerospace and complex operations, directly into your AI workflow. Manage your operational procedures and checklists, track real-time procedure runs and executions, monitor flagged issues and discrepancies, and oversee your technical projects using natural language.

### What you can do

- **Procedure Oversight** — List and retrieve detailed settings, versions, and safety protocols for all your operational procedures.
- **Execution Intelligence** — Monitor active procedure runs, resolving real-time progress, operator inputs, and completed steps.
- **Discrepancy Management** — Access and monitor flagged issues during executions, identifying severity levels and required actions.
- **Operations Auditing** — Retrieve high-level summaries of procedure volume, run success rates, and organizational operational health.

### How it works

1. Connect the Epsilon3 integration to your AI assistant.
2. Authorize using your Epsilon3 API Key (found in your account settings).
3. Orchestrate your complex operations and technical procedures through intuitive conversation.

### Who is this for?

- **Operations Managers** — Quickly check procedure run progress and flagged issues on the go.
- **Technical Engineers** — Research specific procedure versions and execution telemetry via chat during testing.
- **Safety & Quality Teams** — Monitor compliance with safety protocols and organizational operational metadata instantly.


## Available Tools
- **list_latest_procedure_executions**: Identify the most recently started or completed procedure runs
- **get_run_execution_telemetry**: Get detailed execution data and telemetry for a specific procedure run
- **list_successfully_completed_runs**: Identify procedure runs that have reached a "Completed" status
- **list_operations_flagged_issues**: List all issues and discrepancies flagged during procedure runs
- **list_active_procedure_runs**: List all active and historical procedure runs/executions
- **get_epsilon3_account_metadata**: Retrieve metadata and limits for your Epsilon3 account
- **get_procedure_detailed_content**: Get detailed settings and steps for a specific procedure
- **quick_operations_health_audit**: Retrieve a high-level summary of procedures and active runs
- **list_operations_procedures**: List all operational procedures configured in your Epsilon3 account
- **list_aerospace_projects**: List all high-level projects managed in Epsilon3


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Epsilon3 Aerospace Operations** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active procedure runs."

**🤖 AI Agent:**
> I've found 3 active runs, including 'Pre-Launch Checklist' (Run #102) and 'Engine Test Protocol' (Run #105). Run #102 is currently at step 15/40. Would you like the full telemetry for the Engine Test?

---

**👤 You:**
> "Show me procedures for the 'Satellite-A' project."

**🤖 AI Agent:**
> For project 'Satellite-A', I've retrieved 5 procedures, including 'Solar Array Deployment' and 'Battery Health Check'. Both are in version 2.1. Should I pull the detailed steps for Solar Array Deployment?

---

**👤 You:**
> "Were there any issues flagged during today's runs?"

**🤖 AI Agent:**
> Yes, 2 issues were flagged today: 'Sensor Calibration Delay' (Severity: Low) during Run #105 and 'Pressure Variance' (Severity: Medium) during Run #108. Would you like the operator comments for the Pressure Variance issue?


## Installation & Usage

To install and use the **Epsilon3 Aerospace Operations** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/epsilon3-aerospace-operations](https://vinkius.com/mcp/epsilon3-aerospace-operations)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
