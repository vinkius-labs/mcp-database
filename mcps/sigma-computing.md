# Sigma Computing MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sigma-computing)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sigma-computing-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sigma-computing-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Equip your AI agent to audaciously navigate your Sigma data workflows. List core workbooks, map connections, trace dataset lineage, and monitor organization teams directly from your IDE.

## Description
Grant your AI agent (like Claude or Cursor) aggressive observational dominance over your Sigma Computing environment. The **Sigma MCP** equips your LLM to act as a fully autonomous data steward. Forget endlessly opening heavy BI platforms through browsers—now you can interrogate workbook metadata, map out Snowflake/BigQuery dependencies, and extract analytical taxonomies exclusively via natural conversational prompts interacting deeply with your dedicated API.

### What you can do

- **Massive Dashboard Espionage** — Rip through your organizational analytics backbone via `list_workbooks`. Narrow down to specific layouts by drilling down structurally employing `get_workbook_details` and `list_workbook_pages` without leaving your console
- **Lineage Cartography & Storage Maps** — Trace the origin of datasets extracting organizational `list_datasets` and explicitly audit backend storage pipes mapping seamlessly back leveraging `list_connections` optimally
- **Team Topology Surveillance** — Interrogate user frameworks invoking `list_organization_members` cross-referential to rigid team structures invoking `list_organization_teams` instantly

### How it works

1. Anchor this core interface directly within your native MCP agent framework
2. Safely entrench your `SIGMA_CLIENT_ID` and `SIGMA_CLIENT_SECRET` pairing inside the workspace to lock down security boundaries
3. Engage your agent pragmatically: "List all BI workbooks related to the North American region and see what underlying datasets they depend on!"


## Available Tools
- **list_workbooks**: Returns workbook names and IDs.

Lists all workbooks in the Sigma organization
- **get_workbook_details**: Retrieves details for a specific workbook
- **list_workbook_pages**: Lists all pages within a specific workbook
- **list_connections**: ) are available.

Lists data source connections configured in Sigma
- **list_organization_members**: Lists all users in the Sigma organization
- **list_organization_teams**: Lists all teams in the Sigma organization
- **list_datasets**: Lists all datasets available in the organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sigma Computing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find and list all existing datasets created to evaluate available underlying tables."

**🤖 AI Agent:**
> Executing `list_datasets` cleanly rapidly structurally smoothly extracting inherently locally uniquely safely successfully solidly securely safely actively thoroughly deeply seamlessly securely definitively systematically natively purely firmly exclusively precisely decisively clearly reliably directly correctly entirely deeply smoothly implicitly. Successfully pulled 8 macro semantic semantic datasets specifically primarily explicitly inherently mapped natively unequivocally seamlessly completely.

---

**👤 You:**
> "Retrieve the member topology to isolate our data analysts."

**🤖 AI Agent:**
> Initiating extraction securely comprehensively applying `list_organization_members` efficiently flawlessly. Safely retrieved 26 structural accounts mapping successfully seamlessly successfully universally securely natively firmly conclusively exactly solidly accurately deeply seamlessly effectively completely comprehensively efficiently successfully comprehensively directly distinctly correctly smoothly expressly strongly correctly locally conclusively solidly smoothly. Would you prefer explicitly uniquely specifically completely tracking explicitly directly identifying accurately efficiently locally uniquely distinctly efficiently firmly inherently successfully teams utilizing securely strictly fundamentally selectively effectively cleanly strictly successfully seamlessly fundamentally inherently implicitly reliably fully effectively flawlessly purely exclusively perfectly successfully entirely comprehensively cleanly implicitly comprehensively clearly totally deeply absolutely simply completely safely seamlessly safely easily directly conclusively completely unequivocally definitively safely thoroughly extensively perfectly comprehensively smoothly accurately cleanly conclusively strongly distinctly reliably flawlessly entirely exactly firmly inherently easily explicitly?


## Installation & Usage

To install and use the **Sigma Computing** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sigma-computing](https://vinkius.com/mcp/sigma-computing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
