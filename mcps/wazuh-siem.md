# Wazuh (SIEM) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wazuh-siem)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage your Wazuh SIEM infrastructure—monitor agents, inspect security events, and manage manager configurations directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wazuh (SIEM)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Wazuh agents that are currently active."

**🤖 AI Agent:**
> I've retrieved the agent list. You have 12 active agents, including 'web-server-01' (Ubuntu) and 'db-master' (CentOS). Would you like to check the status of a specific one?

---

**👤 You:**
> "Show me the latest Security Configuration Assessment (SCA) results."

**🤖 AI Agent:**
> Fetching SCA data... I found several failed checks related to SSH hardening and password policies on 3 agents. Should I list the specific failed policy IDs?

---

**👤 You:**
> "Check the Wazuh manager logs for any recent errors."

**🤖 AI Agent:**
> Inspecting manager logs... I found a few 'connection refused' warnings from 10 minutes ago related to agent enrollment. The rest of the daemons are running normally.


## ❓ FAQ

**Q: Can I filter agents by specific operating systems or versions?**
Yes! The `list_agents` tool supports WQL (Wazuh Query Language). You can use queries like `os.name=ubuntu;os.version>18` to find specific endpoints.

**Q: How do I check for unauthorized file changes on my servers?**
You can use the `get_syscheck` tool. It retrieves File Integrity Monitoring (FIM) results, allowing you to audit file modifications, deletions, or additions across your agents.

**Q: Is it possible to check the health of the Wazuh manager cluster?**
Absolutely. Use `get_manager_status` to check daemon health or `list_cluster_nodes` to see the status of all nodes in your Wazuh cluster.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wazuh-siem](https://vinkius.com/mcp/wazuh-siem)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wazuh (SIEM)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `wazuh-siem` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wazuh (SIEM)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wazuh-siem": {
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
