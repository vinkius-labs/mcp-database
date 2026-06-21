# OFAC Sanctions Service MCP Server

Access authoritative sanctions data via OFAC SLS — track SDN lists, entities, and version history directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ofac-sanctions-service)

## Overview
**Category:** the-unthinkable
**Tools Count:** 10

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


## Installation & Usage

To install and use the **OFAC Sanctions Service** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ofac-sanctions-service](https://vinkius.com/mcp/ofac-sanctions-service)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
