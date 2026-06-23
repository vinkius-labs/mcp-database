# Kibana MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kibana)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Manage Kibana spaces and saved objects—list dashboards, search index patterns, and organize your observability stack directly from any AI agent.

## Description
Connect your **Kibana** instance to any AI agent to streamline your Elastic Stack management and observability workflows through natural language.

### What you can do

- **Space Management** — List, create, and inspect Kibana spaces to organize your dashboards and visualizations across different teams or environments.
- **Saved Objects Discovery** — Search for dashboards, index patterns, and visualizations using specific queries or types across your instance.
- **Object Portability** — Copy saved objects between different spaces to maintain consistency across your monitoring environments.
- **Deep Inspection** — Retrieve full metadata and attributes for specific saved objects to understand their configuration without manual navigation.
- **Lifecycle Control** — Create, update, or delete spaces and saved objects to automate the setup of your observability stack.

### How it works

1. Subscribe to this server
2. Provide your Kibana URL and a valid API Key
3. Start managing your Elastic environments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & SREs** — quickly audit space configurations and move dashboards between staging and production environments.
- **Data Analysts** — find specific visualizations or index patterns across massive Kibana instances using natural language search.
- **Platform Engineers** — automate the provisioning of team-specific spaces and default saved objects.


## Available Tools (55)
- **add_case_comment**: Add a comment to a case
- **bulk_create_saved_objects**: Create multiple saved objects
- **bulk_get_saved_objects**: Get multiple saved objects
- **bulk_update_saved_objects**: Update multiple saved objects
- **copy_saved_objects**: Copy saved objects between spaces
- **create_agent_policy**: Create an agent policy
- **create_case**: Create a case
- **create_connector**: Create a connector
- **create_data_view**: Create a data view
- **create_enrollment_key**: Create an enrollment key
- **create_or_update_role**: Create or update a Kibana role
- **create_rule**: Create an alerting rule
- **create_runtime_field**: Create or update a runtime field in a data view
- **create_saved_object**: Create a saved object
- **create_short_url**: Create a short URL
- **create_space**: Create a new Kibana space
- **delete_cases**: Delete cases
- **delete_connector**: Delete a connector
- **delete_data_view**: Delete a data view
- **delete_role**: Delete a Kibana role
- **delete_rule**: Delete an alerting rule
- **delete_saved_object**: Delete a saved object
- **delete_short_url**: Delete a short URL
- **delete_space**: Delete a Kibana space
- **disable_rule**: Disable an alerting rule
- **enable_rule**: Enable an alerting rule
- **execute_connector**: Run a connector action
- **export_saved_objects**: Export sets of saved objects
- **find_rules**: Find alerting rules
- **find_saved_objects**: Search for saved objects
- **get_agent**: Get Elastic Agent details
- **get_case**: Get case details
- **get_connector**: Get connector details
- **get_data_view**: Get a specific data view
- **get_role**: Get a specific Kibana role
- **get_rule**: Get alerting rule details
- **get_saved_object**: Get a specific saved object
- **get_short_url**: Get details for a short URL
- **get_space**: Get details for a specific Kibana space
- **import_saved_objects**: Import saved objects from a file
- **list_agent_policies**: List agent policies
- **list_agents**: List Elastic Agents
- **list_connectors**: Get all connectors
- **list_data_views**: Get all data views
- **list_enrollment_keys**: List enrollment keys
- **list_roles**: Get all Kibana roles
- **list_spaces**: Get all Kibana spaces
- **resolve_import_errors**: Resolve errors during import
- **search_cases**: Search cases
- **unenroll_agent**: Unenroll an Elastic Agent
- **update_cases**: Update cases
- **update_data_view**: Update a data view
- **update_rule**: Update an alerting rule
- **update_saved_object**: Update a saved object
- **update_space**: Update an existing Kibana space


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kibana** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available Kibana spaces."

**🤖 AI Agent:**
> I've retrieved the spaces. You have 3 spaces: 'Default', 'Engineering-Logs' (ID: eng-logs), and 'Security-Ops' (ID: sec-ops).

---

**👤 You:**
> "Find all dashboards related to 'Network Traffic' in the 'Default' space."

**🤖 AI Agent:**
> Searching... I found 2 dashboards: 'Global Network Traffic Overview' (ID: net-01) and 'VPC Flow Logs Analysis' (ID: vpc-02). Would you like the details for one of them?

---

**👤 You:**
> "Get the details for the saved object of type 'index-pattern' with ID 'logs-*'."

**🤖 AI Agent:**
> Fetching object... The index pattern 'logs-*' is configured with the time field '@timestamp' and contains 45 mapped fields. It was last updated on 2023-10-25.


## ❓ FAQ

**Q: Can I search for a specific dashboard across my entire Kibana instance?**
Yes. Use the `find_saved_objects` tool and specify the type as 'dashboard'. You can also provide a search string to filter the results by name or description.

**Q: Is it possible to move dashboards from a development space to a production space?**
Absolutely. The `copy_saved_objects` tool allows you to select objects from a source space and replicate them into one or more target spaces, including their references.

**Q: Can I create new Kibana spaces using this integration?**
Yes, you can use the `create_space` action. You just need to provide the space configuration JSON, including the ID and name you want for the new environment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kibana](https://vinkius.com/mcp/kibana)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kibana** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kibana` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kibana** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kibana": {
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
