# Celoxis MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/celoxis)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/celoxis-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/celoxis-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Empower your AI agents to manage complex portfolios, track project milestones, and analyze resource timesheets on Celoxis.

## Description
Connect your **Celoxis** enterprise platform to any AI agent and take full control of your Project Portfolio Management (PPM) workflow through natural conversation.

### What you can do

- **Project & Portfolio Mapping** — List strategic portfolios and extract granular project structures including absolute timelines, completion statuses, and mapped budget blocks.
- **WBS & Tasks** — Retrieve explicit Work Breakdown Structure nodes, identifying active assignments, task health, and explicit phase deliverables.
- **Resource Allocation** — Evaluate working resources, parse user mappings, and expose global scheduling types and distinct system roles across your organization.
- **Timesheets & Accounting** — Accurately pull time entries logged by members to measure billable matrices and ledger associations tied directly to tasks natively.
- **Issue & Risk Governance** — Poll blocking issues preventing workflows and assess graded severity impacts modeled inside the Celoxis organizational risk matrix.
- **Approvals Pipeline** — Interrogate pending validations routing over timesheets, assessing gating rules and internal clearance statuses immediately.

### How it works

1. Subscribe to this server
2. Provide your Celoxis instance Base URL alongside your API Token
3. Start fetching intricate project lifecycles and team burn-rates securely without touching Gantt charts

### Who is this for?

- **Project Managers (PMO)** — Command your custom agent to generate a rapid textual brief regarding delayed milestones affecting priority client accounts.
- **Financial Controllers** — Assess timesheet gaps and non-billable raw expenses mapping accurately directly to current CRM portfolios.
- **Executive Operations** — Ask the model to pull broad Strategic global Portfolios ensuring the pipeline moves correctly around distinct delivery phases.


## Available Tools
- **list_projects**: List all top-level project portfolio items in Celoxis. Returns physical IDs, names, status, and timeline data
- **get_project**: Get an explicit Celoxis project and its complete intrinsic properties structure by ID
- **list_tasks**: List comprehensive Work Breakdown Structure (WBS) tasks representing concrete deliverables within active projects
- **list_resources**: List all explicit Celoxis working resources parsing the core user mappings handling allocations
- **list_time_entries**: List actual time entries logged explicitly against Celoxis tasks or projects for accounting
- **list_issues**: List custom app items representing blocked issues explicit to complex workflows mapping problems
- **list_risks**: List explicit organizational risks bounded natively via the Celoxis custom application matrix
- **list_expenses**: List raw billable/non-billable expenses physically mapped onto task items inside the ecosystem
- **list_clients**: List explicit top-level CRM organizational clients linked internally to distinct portfolios
- **list_portfolios**: List strategic global tracking Portfolios mapping top-level aggregates over child projects natively
- **list_milestones**: List raw milestones natively mapping absolute phase delivery tracking inside the WBS
- **list_approvals**: List explicit tracking objects identifying pending/cleared approvals over timesheets and expenses constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Celoxis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in our company portfolio and check their timeline status."

**🤖 AI Agent:**
> The query executed successfully traversing the portfolios. Your domain houses 6 main active structures. The 'Mobile App Revamp' project is unfortunately marked 'At Risk' structurally due to past-due milestones, whereas 'Data Pipeline Q4' is progressing 'On Track'. I can pull the delayed task elements if you request.

---

**👤 You:**
> "Check the detailed logged time entries for the Marketing project and verify pending approvals."

**🤖 AI Agent:**
> Scanning timesheet nodes… The 'Marketing V2' project has 180 entries logged cumulatively this quarter. I cross-referenced the approval endpoints and isolated 4 distinct entries from John Doe lingering implicitly without organizational clearance. Would you like the ledger of those distinct rows?

---

**👤 You:**
> "Extract the explicit risk logs and blocked issues reported across our client portfolio."

**🤖 AI Agent:**
> I've pulled the risks matrices mapping your global network structures. There are 2 high-severity systemic risks graded heavily impacting the standard client CRM deliveries, notably a 'Supply Bottleneck' bound to the primary client entity mapping. Should I extract the isolated blocking tasks mapped there as well?


## Installation & Usage

To install and use the **Celoxis** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/celoxis](https://vinkius.com/mcp/celoxis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
