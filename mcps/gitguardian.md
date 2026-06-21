# GitGuardian MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gitguardian)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gitguardian-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gitguardian-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Automate secret detection and incident response via GitGuardian — manage secret incidents, deploy honeytokens, and audit workspace security directly from your AI agent.

## Description
Connect your **GitGuardian** workspace to any AI agent to strengthen your security posture and manage secret leaks through natural conversation.

### What you can do

- **Incident Management** — List, retrieve, and resolve secret incidents. Assign team members to leaks and track remediation progress.
- **Honeytokens** — Create and manage decoy credentials (honeytokens) to detect unauthorized access to your private infrastructure.
- **Security Scanning** — Scan code snippets or content for secrets and sensitive data in real-time to prevent leaks before they happen.
- **Audit & Compliance** — Access detailed audit logs to monitor workspace activity and ensure compliance with security policies.
- **Team Collaboration** — Manage teams, members, and API tokens to orchestrate security operations across your organization.

### How it works

1. Subscribe to this server
2. Enter your GitGuardian API Key
3. Start monitoring and securing your code from Claude, Cursor, or any MCP-compatible client

Your AI acts as a 24/7 Security Operations Center (SOC) assistant, helping you triage alerts and deploy defenses without leaving your workflow.

### Who is this for?

- **Security Engineers** — quickly triage secret incidents and manage honeytoken deployments across multiple environments.
- **DevOps & SREs** — automate security audits and monitor workspace health checks directly from the terminal or IDE.
- **Developers** — scan code for secrets before committing and check incident statuses without switching to the GitGuardian dashboard.


## Available Tools
- **assign_secret_incident**: Assign a secret incident
- **bulk_prefix_lookup**: Bulk lookup for honeytoken HMSL hashes
- **create_custom_tag**: Create a custom tag
- **create_honeytoken_note**: Create a honeytoken note
- **create_honeytoken**: Create a honeytoken
- **create_honeytoken_with_context**: Create a honeytoken within a context
- **create_team**: Create a team
- **delete_custom_tag**: Delete a custom tag
- **delete_custom_tags_key**: Delete a custom tags key
- **get_custom_tag**: Retrieve a custom tag
- **get_health**: Check API health status
- **get_honeytoken**: Retrieve a honeytoken
- **get_quotas**: Retrieve quota overview
- **get_secret_incident**: Retrieve secret incident details
- **get_self_api_token**: Retrieve current API token details
- **ignore_secret_incident**: Ignore a secret incident
- **list_api_tokens**: List API tokens
- **list_audit_log_event_names**: List all existing event names for audit logs
- **list_audit_logs**: List audit logs for your workspace
- **list_custom_tags**: List custom tags
- **list_health_check_history**: List health check history for an instance
- **list_health_checks**: List health checks
- **list_honeytoken_events**: List all honeytokens events
- **list_honeytoken_notes**: List honeytoken notes
- **list_honeytoken_sources**: List sources where a honeytoken appears
- **list_honeytokens**: List honeytokens
- **list_ip_allowlist**: List IP allowlist rules
- **list_ips**: List GitGuardian's own IP addresses
- **list_members**: List workspace members
- **list_scim_groups**: List groups via SCIM
- **list_scim_users**: List members via SCIM
- **list_secret_incidents**: List secret incidents
- **list_sources**: List all sources
- **list_team_memberships**: List team members
- **list_teams**: List teams
- **multiscan_content**: Scan multiple contents for secrets
- **reset_honeytoken**: Reset a honeytoken
- **resolve_secret_incident**: Resolve a secret incident
- **revoke_honeytoken**: Revoke a honeytoken
- **revoke_self_api_token**: Revoke current API token
- **scan_and_create_incidents**: Scan content and create incidents automatically
- **scan_content**: Scan content for secrets
- **trigger_health_check**: Trigger a health check
- **trigger_source_scans**: Trigger scans on sources
- **update_custom_tag_full**: Full update of a custom tag
- **update_custom_tag_partial**: Partial update of a custom tag
- **update_custom_tags_key**: Update a custom tags key
- **update_honeytoken**: Update a honeytoken
- **update_secret_incident**: Update a secret incident


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GitGuardian** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent secret incidents in my workspace."

**🤖 AI Agent:**
> I've retrieved the latest incidents. There are 3 active leaks: a 'GitHub Personal Access Token' in repository 'web-app' and two 'AWS Keys' in 'legacy-service'. Would you like the details for the GitHub token leak?

---

**👤 You:**
> "Create a new AWS honeytoken named 'Internal-Dev-Decoy'."

**🤖 AI Agent:**
> Successfully created the honeytoken 'Internal-Dev-Decoy'. The AWS Access Key ID is `AKIA...` and the Secret Key is provided in the metadata. You can now place this in your environment to detect intruders.

---

**👤 You:**
> "Scan this code for secrets: 'const apiKey = "sk_live_51MzX..."'"

**🤖 AI Agent:**
> Scan complete. I detected a 'Stripe Live Secret Key' in the provided string. This is a high-severity finding. I recommend rotating this key immediately and removing it from your source code.


## Installation & Usage

To install and use the **GitGuardian** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gitguardian](https://vinkius.com/mcp/gitguardian)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
