# PlanetScale MCP Server

Provision, branch, and manage serverless MySQL databases dynamically via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/planetscale)

## Overview
**Category:** loved-by-devs
**Tools Count:** 10

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


## Installation & Usage

To install and use the **PlanetScale** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/planetscale](https://vinkius.com/mcp/planetscale)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
