# Terraform Cloud (HCP) MCP Server

Manage infrastructure lifecycle via Terraform Cloud (HCP) — list organizations, manage workspaces, trigger runs, and inspect state outputs directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/terraform-cloud-hcp)

## Overview
**Category:** ship-it
**Tools Count:** 42

## Description
Connect your **Terraform Cloud (HCP)** account to any AI agent to orchestrate your Infrastructure as Code (IaC) workflows through natural language. This server provides comprehensive access to the HCP Terraform API, allowing for seamless management of the entire infrastructure lifecycle.

### What you can do

- **Organization & Project Management** — List, create, and inspect organizations and projects to maintain high-level governance.
- **Workspace Operations** — Query workspaces, manage locks, and configure VCS integrations for automated deployments.
- **Run & Plan Lifecycle** — Trigger new runs, apply or discard plans, and monitor the progress of infrastructure changes in real-time.
- **State & Outputs** — Retrieve current state versions and extract specific output values to use in downstream automation or analysis.
- **Governance & Security** — Manage teams, access controls, variable sets, and Sentinel/OPA policies directly via the agent.

### How it works

1. Subscribe to this server
2. Enter your Terraform Cloud User or Team API Token
3. Start managing your cloud environments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & Platform Engineers** — automate routine workspace management and run monitoring without leaving the terminal or chat.
- **Cloud Architects** — quickly inspect state outputs and policy compliance across multiple organizations.
- **SRE Teams** — troubleshoot failed runs and manage workspace locks during incident response.


## Available Tools
- **add_team_user**: Add a user to a team
- **add_team_workspace_access**: Grant a team access to a workspace
- **apply_run**: Apply a planned run
- **apply_variable_set_to_workspace**: Apply a variable set to a workspace
- **associate_run_task_to_workspace**: Associate a run task with a workspace
- **cancel_run**: Cancel a run
- **create_notification_configuration**: Create a notification configuration for a workspace
- **create_organization**: Create a new organization
- **create_policy_set**: Create a policy set
- **create_policy**: Create a policy
- **create_project**: Create a new project
- **create_registry_module**: Create a private registry module (No VCS)
- **create_registry_provider**: Create a private registry provider
- **create_run_task**: Create a run task
- **create_run**: Create a new run (plan/apply)
- **create_state_version**: Create a new state version
- **create_team**: Create a new team
- **create_variable_set**: Create a variable set
- **create_workspace**: Create a new workspace
- **create_workspace_variable**: Create a variable in a workspace
- **destroy_organization**: Destroy an organization
- **discard_run**: Discard a run
- **explorer_query**: Execute an explorer query across workspaces
- **force_unlock_workspace**: Force unlock a workspace
- **get_current_state_version**: Get current state version for a workspace
- **get_plan_json**: Get JSON execution plan output
- **get_state_version_outputs**: Get outputs for a state version
- **list_audit_events**: List organization audit events
- **list_organizations**: List HCP Terraform organizations
- **list_projects**: List projects in an organization
- **list_teams**: List teams in an organization
- **list_workspaces**: List workspaces in an organization
- **lock_workspace**: Lock a workspace
- **remove_team_user**: Remove a user from a team
- **safe_delete_workspace**: Safe delete a workspace
- **show_apply**: Show details of an apply
- **show_organization**: Show details of a specific organization
- **show_plan**: Show details of a plan
- **unlock_workspace**: Unlock a workspace
- **update_organization**: Update an existing organization
- **update_team**: Update a team
- **upload_policy_code**: Upload code for a policy


## Installation & Usage

To install and use the **Terraform Cloud (HCP)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/terraform-cloud-hcp](https://vinkius.com/mcp/terraform-cloud-hcp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
