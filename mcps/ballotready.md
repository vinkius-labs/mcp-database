# BallotReady MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ballotready)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Civic data and election information — track upcoming elections, candidates, and districts via AI.

## Description
Empower your AI agent to navigate the complex landscape of civic engagement with **BallotReady**, the leading platform for nonpartisan election information. By connecting BallotReady to your agent, you transform dense voter data into a natural conversation. Your agent can instantly identify upcoming local, state, and national elections based on a specific address, retrieve detailed candidate profiles, audit voting districts, and even explain ballot measures without you ever searching through government portals. Whether you're building a voter outreach tool or a civic dashboard, your agent acts as a direct, reliable bridge to the democratic process.

### What you can do

- **Election Discovery** — Find all upcoming elections (local, state, and federal) based on any physical address in the United States.
- **Candidate Profiling** — Retrieve comprehensive profiles for candidates running for office, including their positions and bios.
- **District Mapping** — Instantly match any address to its specific voting districts to understand local representation.
- **Ballot Insights** — Access and explain specific ballot measures and referendums for upcoming elections directly from chat.
- **Officeholder Auditing** — List current officeholders for specific districts to maintain an accurate view of elected leadership.

### How it works

1. Subscribe to this server
2. Enter your BallotReady API Key
3. Start exploring civic and election data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Civic Organizations** — automate voter information retrieval and outreach campaigns through natural language.
- **Political Researchers** — audit candidate backgrounds and election schedules across multiple jurisdictions efficiently.
- **Non-Profit Teams** — build AI-driven civic engagement tools to help communities understand their local ballots.
- **News & Media** — quickly retrieve accurate, nonpartisan election data for reporting and fact-checking.


## Available Tools (10)
- **get_account_check**: Verify BallotReady connection
- **get_ballot_measures**: Retrieve ballot measures for a specific election
- **list_positions**: List specific offices up for election
- **get_candidate**: Get detailed profile for a specific candidate
- **get_districts_by_address**: Convenience tool to get districts by address
- **get_elections_by_address**: Convenience tool to get elections by address
- **get_officeholders**: Retrieve current officeholders for districts
- **list_candidates**: List candidates running for office
- **list_districts**: Match an address to specific voting districts
- **list_elections**: Find upcoming elections based on a specific address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BallotReady** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What elections are coming up for the address 123 Main St, Chicago, IL?"

**🤖 AI Agent:**
> I've found 2 upcoming elections for that address: the General Election on November 3rd and a Municipal Special Election on June 15th. Would you like to see the candidates or ballot measures for either?

---

**👤 You:**
> "Show me the profile for candidate ID 98765."

**🤖 AI Agent:**
> Candidate Profile: Jane Smith. She is running for State Senate. Her platform focuses on education reform and infrastructure. I can provide more details on her previous experience if needed.

---

**👤 You:**
> "Which voting districts cover 1600 Pennsylvania Ave NW, Washington, DC?"

**🤖 AI Agent:**
> Retrieving district mapping... That address is covered by DC's At-Large Congressional District and DC Council Ward 2. I can also list the current officeholders for these districts.


## ❓ FAQ

**Q: Can I search for elections using just a city name?**
For the highest accuracy, BallotReady tools like `list_elections` require a specific physical address (Street, City, State, ZIP). This ensures the agent returns the exact ballot measures and candidates for that specific location.

**Q: Does this integration provide information for international elections?**
Currently, BallotReady focuses exclusively on comprehensive civic data within the United States, including local, state, and federal contests.

**Q: Can the agent tell me who my current representatives are?**
Yes. Use the `get_officeholders` tool by providing a district ID (retrieved via `list_districts` for an address) to see a list of current leaders representing that area.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ballotready](https://vinkius.com/mcp/ballotready)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BallotReady** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ballotready` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BallotReady** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ballotready": {
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
