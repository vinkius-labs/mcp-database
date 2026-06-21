# OFAC Sanctions Service MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ofac-sanctions-service)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ofac-sanctions-service-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ofac-sanctions-service-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access authoritative sanctions data via OFAC SLS — track SDN lists, entities, and version history directly from your AI agent.

## Description
Connect to the **OFAC Sanctions List Service (SLS)** API through your AI agent and explore authoritative data on sanctioned individuals, groups, and entities using natural conversation.

### What you can do

- **List Discovery** — Retrieve identifiers for all available sanctions lists, including the Specially Designated Nationals (SDN) and Consolidated Non-SDN lists.
- **Update Monitoring** — Check the timestamp of the last update for any sanctions list to ensure you are using the most current data.
- **Version Tracking** — List historical and current versions of sanctions lists and retrieve specific version metadata.
- **Entity Inspection** — Access detailed profile information for specific sanctioned entities, including names, aliases, and addresses.
- **Deltas & Full Versions** — Retrieve metadata for full list versions or just the changes (deltas) between specific versions.
- **Entry Metrics** — Get the total count of entities within a specific list version for audit purposes.
- **Tag Management** — List all descriptive tags and labels associated with list versions.

### How it works

1. Subscribe to this server
2. (Optional) Enter your OFAC SLS API Key
3. Start exploring sanctions intelligence from Claude, Cursor, or any MCP client

### Who is this for?

- **Compliance Officers** — quickly verify entity details or list updates without manually downloading large files.
- **Legal Teams** — monitor for new additions to the SDN list directly from your workspace.
- **Risk Analysts** — automate the retrieval of version metadata and entry counts for compliance reporting.


## Available Tools
- **get_sls_about**: Get SLS API info
- **get_delta_version_metadata**: Get delta version metadata
- **get_entity_details**: Get specific entity metadata
- **get_version_entry_count**: Get total entries in a version
- **get_full_version_metadata**: Get full version metadata
- **get_list_last_updated**: Check for list updates
- **list_version_entities**: List entities in a version
- **list_sanctions_lists**: g. SDN, NONSDN).

List available sanctions lists
- **list_version_tags**: List tags for a version
- **list_list_versions**: List versions of a sanctions list


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OFAC Sanctions Service** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "When was the SDN sanctions list last updated?"

**🤖 AI Agent:**
> Checking update status... The SDN sanctions list was last updated today at 10:15 AM UTC. Would you like to see the entry count for the latest version?

---

**👤 You:**
> "Get the details for entity ID '12345' in the latest SDN version."

**🤖 AI Agent:**
> Inspecting entity 12345... This record belongs to 'Example Global Group'. It has 3 known aliases and is associated with 2 addresses in Zurich. Shall I retrieve the full version metadata for this list?

---

**👤 You:**
> "List all historical versions available for the SDN list."

**🤖 AI Agent:**
> Retrieving version history... I found 12 historical versions for the SDN list, ranging from January 2023 to the current version published today. Would you like to check the delta (changes) between the last two versions?


## Installation & Usage

To install and use the **OFAC Sanctions Service** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ofac-sanctions-service](https://vinkius.com/mcp/ofac-sanctions-service)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
