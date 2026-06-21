# Runlayer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/runlayer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

AI enterprise control plane: manage MCP servers, skills, agents, and security policies via agents.

## Description
### What you can do

Connect AI agents to the Runlayer Enterprise Control Plane for comprehensive MCP ecosystem management:

- **Manage MCP Servers** — register, inspect, update, and remove serverless MCP endpoints
- **Manage Skills** — create, assign, and version reusable agent capabilities
- **Manage Agents** — onboard AI agents (Claude, Cursor, VS Code, custom) with proper security guardrails
- **Enforce Policies** — define and audit security policies governing MCP access and agent permissions
- **Audit Everything** — retrieve complete audit trails of all MCP, skill, agent, and policy operations
- **Manage API Keys** — create, rotate, and revoke organization and personal API keys
- **Run Security Scans** — discover shadow AI, unauthorized MCP servers, and policy violations across your organization
- **Monitor Organization Health** — review member activity, server inventory, and security posture

### How it works

1. **Generate an Organization API Key** from Runlayer dashboard (Settings > API Keys)
2. **Configure your Runlayer host URL** (your organization's Runlayer instance)
3. **Ask your AI agent** to manage servers, enforce policies, audit logs, or discover shadow AI
4. **Natural language commands** replace manual Runlayer dashboard operations

### Who is this for?

Essential for **IT security teams**, **AI governance officers**, **platform engineers**, **compliance managers**, and **enterprise architects** deploying MCP at scale. Let AI agents handle continuous MCP server registration, policy enforcement, audit log review, API key rotation, and shadow AI discovery. Perfect for organizations managing 10+ MCP servers and agents who need to maintain security compliance, prevent unauthorized AI usage, and enable AI-driven infrastructure governance.


## Available Tools
- **create_api_key**: Returns the key value (shown only once) and metadata. Use this to create keys for integrations, CI/CD pipelines, or service accounts. Store the key value securely immediately after creation.

Create a new API key for your Runlayer organization
- **create_agent**: Requires agent name and type (claude_desktop, cursor, vs_code, custom). Optionally assign MCP servers, skills, and policies during registration. Returns the created agent details. Use this to onboard new AI agents to your enterprise control plane with proper security guardrails.

Register a new AI agent in Runlayer
- **revoke_api_key**: This action cannot be undone. Requires the key ID. Use this for compromised keys, unused keys, or during security incidents.

Revoke an API key immediately
- **create_mcp_server**: Requires server name and connection details (URL, authentication method). Optionally assign skills, agents, and policies during registration. Returns the created server details including the new UUID. Use this to onboard new MCP servers to your enterprise control plane.

Register a new MCP server in Runlayer
- **create_policy**: Requires policy name and rule definitions. Returns the created policy. Use this to enforce security standards, restrict access to sensitive MCP servers, or define audit requirements.

Create a new security or access policy in Runlayer
- **create_skill**: Requires skill name and description. Optionally define input/output schemas and initial MCP server assignments. Returns the created skill details. Use this to codify reusable agent capabilities for consistent use across your organization.

Register a new skill (agent capability) in Runlayer
- **delete_agent**: This disconnects the agent from all MCP servers and removes policy assignments. Requires the agent ID. Confirm with the user before proceeding.

Remove an AI agent from Runlayer
- **delete_mcp_server**: This action disconnects all associated agents and removes policy assignments. Requires the server UUID. Confirm with the user before proceeding.

Remove an MCP server from Runlayer
- **delete_policy**: All resources previously governed by this policy will no longer be subject to its rules. Requires the policy ID. Confirm with the user before proceeding.

Remove a security or access policy from Runlayer
- **delete_skill**: Does not delete the underlying MCP server tools. Requires the skill ID. Confirm with the user before proceeding.

Remove a skill from Runlayer
- **get_agent**: Requires the agent ID from list_agents results. Use this to review agent configuration, audit access patterns, or troubleshoot connectivity.

Get detailed information about a specific AI agent
- **get_audit_logs**: Returns timestamps, actor identities, action types, affected resources, and outcomes. Use this for compliance reporting, security investigations, or operational troubleshooting.

Get audit logs for your Runlayer organization
- **get_mcp_server**: Requires the server UUID from list_mcp_servers results. Use this to review server configuration, verify security compliance, or troubleshoot connectivity issues.

Get detailed information about a specific MCP server
- **get_organization**: Use this to verify your organization configuration or get an overview of your MCP ecosystem.

Get your Runlayer organization details
- **get_scan_results**: Requires the scan ID from run_mcp_sweep_scan results. Use this to review shadow AI discoveries, identify policy violations, or generate compliance reports.

Get results from an MCP sweep scan
- **get_skill**: Requires the skill ID from list_skills results. Use this to review skill configuration or understand capability dependencies.

Get detailed information about a specific skill
- **list_api_keys**: Use this to audit key inventory, identify unused keys, or prepare for key rotation.

List all API keys for your Runlayer organization
- **list_agents**: Returns agent names, IDs, types (Claude Desktop, Cursor, custom), assigned MCP servers, active skills, policy compliance status, and last activity timestamps. Use this to understand your agent ecosystem and verify which agents have access to which MCP servers.

List all AI agents registered in your Runlayer organization
- **list_mcp_servers**: Returns server names, UUIDs, status (active, inactive, blocked), assigned skills, connected agents, policy associations, and last activity timestamps. Use this as the first step to understand your MCP server inventory before managing individual servers, applying policies, or reviewing security posture.

List all registered MCP servers in your Runlayer organization
- **list_members**: Use this to audit access, review role assignments, or identify inactive accounts.

List all members of your Runlayer organization
- **list_policies**: Returns policy names, descriptions, enforcement status, affected resources, and violation counts. Use this to review your security posture before creating or modifying policies.

List all security and access policies in your Runlayer organization
- **list_skills**: Returns skill names, descriptions, associated MCP servers, usage counts, and version information. Use this to discover available capabilities before assigning them to agents or MCP servers.

List all skills registered in your Runlayer organization
- **run_mcp_sweep_scan**: Returns a scan ID which can be used with get_scan_results to retrieve findings. Use this for security assessments, compliance audits, or shadow AI detection.

Run an MCP sweep scan to discover shadow AI across your organization
- **update_agent**: Only pass the fields you want to change. Requires the agent ID. Use this to update agent assignments or modify metadata.

Update an existing AI agent configuration
- **update_mcp_server**: Only pass the fields you want to change. Requires the server UUID. Use this to update server endpoints, rotate credentials, or modify policy assignments.

Update an existing MCP server configuration
- **update_policy**: Only pass the fields you want to change. Requires the policy ID. Use this to refine security requirements, update access controls, or modify audit rules.

Update an existing security or access policy
- **update_skill**: Only pass the fields you want to change. Requires the skill ID. Use this to refine skill definitions or update documentation.

Update an existing skill configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Runlayer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all MCP servers registered in our organization and their security status"

**🤖 AI Agent:**
> I'll list all registered MCP servers with their compliance status and policy assignments.

---

**👤 You:**
> "Run a shadow AI discovery scan across our organization and show me the findings"

**🤖 AI Agent:**
> I'll initiate the MCP sweep scan and retrieve all discovered unauthorized resources.

---

**👤 You:**
> "Create a new policy that restricts MCP server access to only approved developers"

**🤖 AI Agent:**
> I'll create a security policy with rules limiting MCP server access to authorized personnel.


## ❓ FAQ

**Q: Do I need a Runlayer enterprise subscription to use this MCP?**
Yes, this MCP server requires an active Runlayer organization with API access. Runlayer is an enterprise-grade control plane, so you need a valid organizational subscription. Contact Runlayer sales to get started and obtain your organization API key.

**Q: Can this MCP server detect unauthorized AI usage (shadow AI)?**
Yes! The run_mcp_sweep_scan tool initiates comprehensive shadow AI discovery across devices, detecting unauthorized MCP servers, OpenClaw installs, Skills, and agents. Results include policy violations and security risks across your organization's endpoints.

**Q: What types of AI agents does Runlayer support?**
Runlayer supports Claude Desktop, Cursor, VS Code with Copilot, Windsurf, and custom AI agents. Each agent type can be registered with specific security policies, assigned MCP servers, and monitored through the audit trail. New agent types can be added as custom integrations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/runlayer](https://vinkius.com/mcp/runlayer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Runlayer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `runlayer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Runlayer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "runlayer": {
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
