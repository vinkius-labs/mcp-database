# Pulumi MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pulumi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage cloud infrastructure via Pulumi — list stacks, track deployments, audit outputs and tag resources from any AI agent.

## Description
Connect your **Pulumi** account to any AI agent and take full control of your infrastructure-as-code through natural conversation.

### What you can do

- **Organization Discovery** — List organizations and retrieve their details, team settings and member info
- **Stack Management** — List, create and delete stacks (infrastructure environments) across all your projects
- **Deployment Tracking** — Monitor stack update history with status (succeeded, failed, in-progress), resource changes and error logs
- **Output Inspection** — View exported output values from the latest deployment (URLs, IPs, resource IDs)
- **Tag Management** — List and set custom tags on stacks for organization and filtering (environment, team, cost-center)

### How it works

1. Subscribe to this server
2. Enter your Pulumi Access Token
3. Start managing your infrastructure from Claude, Cursor, or any MCP-compatible client

No more switching to the Pulumi Console to check deployment status or review stack outputs. Your AI acts as a dedicated infrastructure operations engineer.

### Who is this for?

- **DevOps Engineers** — quickly check stack status, review deployment history and inspect outputs without opening the Pulumi Console
- **Platform Teams** — audit infrastructure changes, track deployment success rates and manage stack tags across organizations
- **Developers** — discover available stacks, review exported endpoints and verify resource provisioning via conversation


## Available Tools
- **create_stack**: A stack is an isolated, independently configurable instance of your Pulumi program. Requires the org name, project name and stack name (e.g. "staging", "prod"). Returns the created stack with its URL.

Create a new Pulumi stack
- **delete_stack**: The stack must be empty (no resources) or force deletion must be enabled. Provide the org name, project name and stack name. WARNING: this action is irreversible.

Delete a Pulumi stack
- **get_current_user**: Returns the user's GitHub login, avatar URL, email and name. Use this to verify your access token is working correctly and to see which identity the API calls will appear as.

Get the currently authenticated Pulumi user
- **get_deployment**: Provide the org name, project name, stack name and deployment version number.

Get details for a specific Pulumi deployment
- **get_organization**: Provide the organization name (slug).

Get details for a specific Pulumi organization
- **get_stack_outputs**: Outputs are values your Pulumi program exports, such as URLs, IP addresses, resource IDs and connection strings. Useful for discovering endpoint addresses and configuration values after infrastructure deployment.

Get the exported output values from a Pulumi stack
- **get_stack**: Provide the org name, project name and stack name.

Get details for a specific Pulumi stack
- **list_deployments**: Each deployment shows its version number, status (succeeded, failed, in-progress), start/end time, resource changes (created, updated, deleted) and the user who triggered it. Use this to audit infrastructure changes and track deployment success/failure patterns.

List deployment history for a Pulumi stack
- **list_stack_tags**: Tags are key-value metadata labels used for organizing, filtering and managing stacks (e.g. environment=prod, team=platform, cost-center=engineering).

List tags on a Pulumi stack
- **list_stacks**: Each stack represents an isolated, independently configurable instance of your infrastructure (e.g. dev, staging, prod). Returns stack name, project name, last update info, resource count and whether updates are in progress.

List all stacks in a Pulumi organization
- **set_stack_tag**: Tags are used for organizing, filtering and managing stacks (e.g. key="environment", value="prod", key="team", value="platform"). Provide the org name, project name, stack name, tag name and tag value.

Set a tag on a Pulumi stack


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pulumi** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all stacks in my organization."

**🤖 AI Agent:**
> I found 6 stacks in your organization: 'my-infra/dev' (last updated 2h ago, 24 resources), 'my-infra/staging' (last updated yesterday, 24 resources), 'my-infra/prod' (last updated 3 days ago, 24 resources), 'networking/prod' (last updated last week, 8 resources), 'database/dev' and 'database/prod' (both created but never updated).

---

**👤 You:**
> "What was the result of the latest deployment to my-infra/prod?"

**🤖 AI Agent:**
> The latest deployment (v12) to my-infra/prod succeeded 3 days ago. It created 2 resources (new S3 bucket and CloudFront distribution), updated 1 resource (EC2 instance type changed) and left 21 unchanged. The deployment took 4 minutes and was triggered by user alice.

---

**👤 You:**
> "Show me the exported outputs from the prod stack."

**🤖 AI Agent:**
> The prod stack exports the following outputs: `api_url: https://api.example.com`, `cdn_url: https://cdn.example.com`, `db_endpoint: postgres://db.example.com:5432`, `s3_bucket_arn: arn:aws:s3:::my-prod-bucket` and `vpc_id: vpc-0abc123`. Would you like details on any of these?


## ❓ FAQ

**Q: How do I get a Pulumi Access Token?**
Log in to the [**Pulumi Console**](https://app.pulumi.com), go to **Account Settings > Access Tokens**, click **Create Token**, give it a name and copy the token immediately — it starts with `pul_` and won't be shown again.

**Q: What is a Pulumi stack?**
A stack is an isolated, independently configurable instance of your Pulumi program. Stacks typically represent different environments like dev, staging and prod. Each stack has its own configuration, state, outputs and deployment history. Use list_stacks to discover all stacks in an organization.

**Q: Can I see the deployment history of a stack?**
Yes! Use `list_deployments` with the org name, project name and stack name. It returns the update history showing version number, status (succeeded, failed, in-progress), start/end time and resource change counts. Use `get_deployment` with a specific version for detailed logs and error messages.

**Q: Can I view the outputs of a stack?**
Yes! Use `get_stack_outputs` with the org name, project name and stack name. It returns all exported output values from the latest successful deployment, such as URLs, IP addresses, resource IDs and connection strings. This is useful for discovering endpoint addresses after infrastructure deployment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pulumi](https://vinkius.com/mcp/pulumi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pulumi** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pulumi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pulumi** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pulumi": {
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
