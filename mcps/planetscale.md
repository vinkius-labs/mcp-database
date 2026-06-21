# PlanetScale MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/planetscale)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Provision, branch, and manage serverless MySQL databases dynamically via AI.

## Description
Empower your AI agents to manage your **PlanetScale** serverless infrastructure seamlessly. Leverage the power of Vitess-backed MySQL without leaving your IDE. Ask your AI to branch a production database for testing, list regions, or drop obsolete schema forks instantly.

### What you can do

- **Database Provisioning** — Instantly list (`list_databases`), inspect, create (`create_database`), or destroy serverless MySQL clusters running across global regions.
- **Branch Management** — Harness PlanetScale's Git-like schema workflows. Direct your LLM to spawn a temporary `shadow-test` branch cloned from `main` (`create_branch`), allowing consequence-free migrations before orchestrating Deploy Requests.
- **Infrastructure Exploration** — Discover strict organizational IDs (`list_organizations`) and query available physical cloud provider edges (`list_regions`) to optimize latency targets.

### How it works

1. Ensure your AI environment has this connector subscribed
2. Provide an active PlanetScale Service Token
3. Manage fleets of serverless data clusters via natural language inside Cursor or Claude

### Who is this for?

- **DevOps Engineers** — automate the destruction of stale staging branches (`delete_branch`) via simple LLM terminal chat commands.
- **Full-stack Developers** — spin up ephemeral database branches for isolated feature development without touching the web console.
- **Platform Architects** — audit distribution footprints, node metadata, and connection strings across multiple organizational environments automatically.


## Available Tools
- **create_branch**: Does *not* duplicate data (creates an empty schema clone of the parent) for secure CI testing uncoupled entirely from `main` load balancing layers.

Fork a PlanetScale schema mapping to a new isolated Branch
- **create_database**: Creates empty environments ready to execute explicit DDL definitions via non-blocking Deploy Requests.

Provision a radically scalable Serverless Database instance
- **delete_branch**: Utilized constantly within CI/CD pipelines following a successful Deploy Request morphing `main` schema structure directly.

Purge an obsolete Git-like Schema testing ground
- **delete_database**: Dropping the database effectively wipes terabytes of records scattered globally. Fails fully if unacknowledged connection logic binds it.

Destroy a PlanetScale MySQL construct irreversibly
- **get_branch**: Returns access hostnames for code integration.

Deconstruct the layout of a single explicit Database Branch
- **get_database**: Analyze core configuration of a specific MySQL cluster logic
- **list_branches**: Essential for migrating schemas without locking production reads/writes.

List Development Database Branches mirroring Prod architectures
- **list_databases**: Retrieves explicitly mapping IDs orchestrating distributed Vitess backend shards.

List high-availability PlanetScale MySQL DB distributions
- **list_organizations**: Used solely to resolve the foundational string key prerequisite for all subsequent MySQL endpoint management.

List root PlanetScale organizational identifiers
- **list_regions**: Critical reference required during new Database/Branch physical provisioning routines.

Locate physical edge availability zones supported by Vitess


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PlanetScale** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all physical cloud regions currently exposed by the PlanetScale integration."

**🤖 AI Agent:**
> I executed `list_regions` successfully against your organization map. I found 15 edge locations. The primary North-American targets are `us-east` (AWS N. Virginia) and `us-west-2` (AWS Oregon). There are also `eu-west` endpoints available for immediate Database generation. Would you like me to create an instance there?

---

**👤 You:**
> "We're starting a new feature. Fork testing branch from the main database 'store-backend'."

**🤖 AI Agent:**
> Executed `create_branch`. Branch `feature-test-1y82` has been successfully spun up under `store-backend`. It copied the exact static schema logic from `main` without migrating standard rows, resulting in an empty, compliant Vitess environment ready for raw testing strings. What's the new DDL injection you're planning?

---

**👤 You:**
> "Drop the specific 'staging-01' branch inside the 'web-portal' database."

**🤖 AI Agent:**
> Command `delete_branch` deployed explicitly specifying target DB 'web-portal' aiming for branch 'staging-01'. The environment hook has been severed internally and queued for complete data physical destruction. Staging-01 operates out of existence as of now.


## ❓ FAQ

**Q: Can I run destructive commands like deleting databases through this AI implementation?**
Yes. The integration provides `delete_branch` and `delete_database`. They map directly to infrastructure teardowns. You should scope the Service Token carefully inside the PlanetScale dashboard to avoid catastrophic misinterpretations if your explicit intent is just testing. Deletions via `delete_database` are absolute and irretrievable.

**Q: Does `create_branch` replicate and copy my production dataset into the new branch?**
No. PlanetScale branches solely duplicate the static underlying DDL structure (schema), exactly like taking a snapshot of empty tables. The new branch boots up free of rows. This design lets your agent freely run `ALTER TABLE` operations independently without crashing the master tables.

**Q: How does the agent know which organizational node I am provisioning my branches on?**
All queries essentially require the foundational string parameters known as the `org_name`. If unknown, a simple `list_organizations` query reveals the UUID scope dictating your authorized account parameter bounds securely.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/planetscale](https://vinkius.com/mcp/planetscale)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PlanetScale** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `planetscale` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PlanetScale** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "planetscale": {
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
