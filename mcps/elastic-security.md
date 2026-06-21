# Elastic Security MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/elastic-security)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/elastic-security-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/elastic-security-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage SIEM and SOC operations via Elastic Security — monitor detection rules, search security alerts (Signals), handle whitelisting, and audit threat coverage directly from any AI agent.

## Description
Connect your **Elastic Security** (SIEM) deployment to any AI agent and take full control of your threat detection and SOC auditing through natural conversation.

### What you can do

- **Detection Rule Orchestration** — List all configured detection rules and retrieve exact EQL or KQL statements to map MITRE ATT&CK coverage natively
- **Live Alert Auditing** — Search raw generated security signals (alerts) consolidating hostname, user profiles, and IP geolocations into a single view
- **Rule Lifecycle Management** — Create new custom log detection rules or irreversibly purge custom logic from the Kibana SIEM engine to tune your environment
- **Exception & Whitelisting** — List global exception lists and whitelist hostnames inside existing containers to resolve false positives and noise in real-time
- **Threat Intel Verification** — Search for specific rules by name, tag, or MITRE tactic to expedite SOC auditing for newly reported CVEs or ransomware
- **State Control** — Enable or disable existing detection rules to manage noisy triggers across large organizational units seamlessly
- **System Health Checks** — Verify if official Elastic prepackaged rules need updates to ensure lack of latest official threat models is addressed

### How it works

1. Subscribe to this server
2. Enter your Kibana Host, Port, and Elastic API Key (found in Kibana > Stack Management > Security > API Keys)
3. Start managing your SIEM operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SOC Analysts** — monitor security alerts and audit detection rules without leaving the chat interface
- **Security Engineers** — create and update detection logic and manage exception lists using natural language
- **CISO & Incident Responders** — quickly search for signals and verify threat coverage during active investigations
- **DevOps Teams** — monitor SIEM health and verify prepackaged rule update statuses in real-time


## Available Tools
- **add_exception**: name value to the target exception container, implicitly ignoring telemetry matched on this field for any rule bound to the list. Use explicitly to resolve false positives.

Whitelist a hostname inside an existing Exception List
- **create_rule**: Defines immediate risk scores multiplying against asset valuations, generating Elastic Signals tracking MITRE TTPs upon match.

Create a new Log Detection Rule tracking malicious Elastic telemetry
- **delete_rule**: Cannot be applied to Elastic Pre-built rules which are managed globally via package updates. Irreversible.

Hard-delete a custom Elastic detection rule completely
- **list_exceptions**: These lists logically bypass specific rules, preventing SIEM alerts from triggering on known-good administrative behavior like vulnerability scanners.

List global exception lists managing detection bypass logic
- **find_detection_rules**: Expedites SOC auditing when evaluating coverage for newly reported CVEs or specific localized threats.

Search for specific Elastic rules by name, tag or MITRE tactic
- **get_rule**: Displays run intervals, severity assignment, index scopes, and explicit reference URLs matching threat intel reports.

Get exact details, intervals, and query logic for a distinct Rule
- **get_prepackaged_rules_status**: Identifies if the environment is lacking the latest official threat models targeting Windows, Linux, and Cloud environments.

Check if official Elastic prepackaged rules need updates
- **list_detection_rules**: g., logs-endpoint*, winlogbeat*). Vital for mapping MITRE ATT&CK coverage against the Elastic schema.

List all detection rules configured within the Elastic SIEM
- **search_signals**: Signals consolidate the triggering payload structure, enriching it with Hostname, User profiles, IP geolocations, and process trees.

Search raw generated Elastic Security alerts (Signals)
- **update_rule**: Used explicitly to disable noisy rules triggering false positives across large organizational units, or to re-enable them post-tuning.

Enable or Disable an existing Elastic Detection Rule


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Elastic Security** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all active detection rules tagged with 'Ransomware'"

**🤖 AI Agent:**
> Searching rules... I found 12 active rules matching 'Ransomware'. Highlights include 'Volume Shadow Copy Deletion via WMIC' and 'Ransomware-linked Process Execution'. Would you like the full logic for any of these?

---

**👤 You:**
> "Add hostname 'dev-machine-01' to exception list 'global-whitelist'"

**🤖 AI Agent:**
> Exception added! 'dev-machine-01' has been whitelisted in 'global-whitelist'. Detection rules bound to this list will now ignore telemetry from this host, resolving the reported false positives.

---

**👤 You:**
> "Search for security signals from user 'admin_root' in the last hour"

**🤖 AI Agent:**
> Retrieving signals for 'admin_root'... I found 2 alerts: 'Suspicious LDAP Query' at 10:15 AM and 'Brute Force Attempt' at 10:45 AM. I can provide the source IP and process tree for these signals.


## Installation & Usage

To install and use the **Elastic Security** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/elastic-security](https://vinkius.com/mcp/elastic-security)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
