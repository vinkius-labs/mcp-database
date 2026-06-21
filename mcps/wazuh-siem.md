# Wazuh (SIEM) MCP Server

Manage your Wazuh SIEM infrastructure—monitor agents, inspect security events, and manage manager configurations directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/wazuh-siem)

## Overview
**Category:** fort-knox
**Tools Count:** 21

## Description
Connect your **Wazuh SIEM** to any AI agent to streamline security operations and endpoint monitoring through natural language.

### What you can do

- **Agent Management** — List all enrolled agents, create new ones, and perform bulk actions like restarts or upgrades using WQL filtering.
- **Manager & Cluster Health** — Monitor manager daemon status, fetch logs, and inspect cluster nodes to ensure high availability.
- **Security Auditing** — Query File Integrity Monitoring (Syscheck), Security Configuration Assessment (SCA), and Rootcheck results.
- **Threat Intelligence** — Access MITRE ATT&CK mappings and test log decoders to validate your detection pipeline.
- **Rule Orchestration** — List and update rules or decoders directly to fine-tune your security posture.

### How it works

1. Subscribe to this server
2. Provide your Wazuh API URL, Username, and Password
3. Start auditing your security environment from Claude, Cursor, or any MCP client

### Who is this for?

- **Security Analysts** — quickly query agent status and FIM results without navigating the Wazuh dashboard
- **DevSecOps Engineers** — automate agent upgrades and monitor cluster health directly from terminal-based AI tools
- **Incident Responders** — fetch MITRE mappings and manager logs instantly during active investigations


## Available Tools
- **list_cluster_nodes**: List Wazuh cluster nodes
- **create_agent**: Enroll a new Wazuh agent
- **create_security_role**: Create a new Wazuh security role
- **list_decoders**: Supports WQL filtering.

List loaded Wazuh decoders
- **delete_agents**: Use WQL to specify which agents to delete.

Remove Wazuh agents
- **list_agents**: Supports WQL filtering.

List all Wazuh agents
- **get_logtest**: Test rules and decoders against logs
- **get_manager_logs**: Retrieve Wazuh manager logs
- **get_manager_status**: Get Wazuh manager daemon status
- **get_mitre**: Supports WQL filtering.

Get MITRE ATT&CK results
- **restart_agents**: Restart Wazuh agents
- **restart_cluster**: Restart the Wazuh cluster
- **get_rootcheck**: Supports WQL filtering.

Get Rootcheck results
- **list_rules**: Supports WQL filtering.

List loaded Wazuh rules
- **get_sca**: Supports WQL filtering.

Get Security Configuration Assessment (SCA) results
- **list_security_users**: List Wazuh API users
- **get_syscheck**: Supports WQL filtering.

Get File Integrity Monitoring (Syscheck) results
- **get_syscollector**: Supports WQL filtering.

Get Syscollector inventory
- **update_rule_file**: Update a Wazuh rule file
- **update_security_config**: Update Wazuh security configuration
- **upgrade_agents**: Upgrade Wazuh agents


## Installation & Usage

To install and use the **Wazuh (SIEM)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wazuh-siem](https://vinkius.com/mcp/wazuh-siem)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
