# Terraform Cloud (HCP) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/terraform-cloud-hcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage infrastructure lifecycle via Terraform Cloud (HCP) — list organizations, manage workspaces, trigger runs, and inspect state outputs directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Terraform Cloud (HCP)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all organizations I have access to in Terraform Cloud."

**🤖 AI Agent:**
> I've found 2 organizations: 'Acme-Corp' and 'Dev-Sandbox'. Which one would you like to explore?

---

**👤 You:**
> "Show me all workspaces in the 'Acme-Corp' organization that have the tag 'production'."

**🤖 AI Agent:**
> Found 3 production workspaces: 'vpc-prod' (ws-K9...), 'eks-main' (ws-L2...), and 'rds-cluster' (ws-M5...).

---

**👤 You:**
> "Get the output values for workspace ws-K9j2L8mP1."

**🤖 AI Agent:**
> The outputs for 'vpc-prod' are: vpc_id = 'vpc-0a1b2c', public_subnets = ['subnet-1', 'subnet-2'], and region = 'us-east-1'.


## ❓ FAQ

**Q: Can I trigger a new infrastructure deployment (run) using this server?**
Yes. You can use the `create_run` tool by providing the Workspace ID. You can also subsequently use `apply_run` or `discard_run` to manage the lifecycle of that specific execution.

**Q: How do I see the output variables from my last successful Terraform apply?**
Use the `get_state_version_outputs` tool with the Workspace ID. It will retrieve all calculated outputs from the current state, such as IP addresses, DNS names, or resource IDs.

**Q: Is it possible to list all workspaces across my organization?**
Absolutely. Use the `list_workspaces` tool and provide your organization name. You can also filter the results by name or tags using optional parameters.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/terraform-cloud-hcp](https://vinkius.com/mcp/terraform-cloud-hcp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Terraform Cloud (HCP)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `terraform-cloud-hcp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Terraform Cloud (HCP)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "terraform-cloud-hcp": {
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
