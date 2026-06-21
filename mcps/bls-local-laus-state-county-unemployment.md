# BLS Local — LAUS State & County Unemployment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bls-local-laus-state-county-unemployment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Explore the Local Area Unemployment Statistics (LAUS) program. Get granular unemployment insights spanning across every US State, County, and Metropolitan Area.

## Description
While other tools look at the USA as a whole, the Local Area Unemployment Statistics (LAUS) MCP provides hyper-localized focus. 

### Included granularity
- **State Level** — Compare California vs Texas.
- **County Level** — Compare Miami-Dade vs Cook County.
- **Metropolitan Statistical Areas (MSAs)**


## Available Tools (1)
- **query_bls**: Use this instead of specific endpoints if you intimately know the underlying numerical code. Up to 50 concurrent lookbacks allowed.

Generic BLS v2 api timeseries query. Requires explicit BLS Series IDs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BLS Local — LAUS State & County Unemployment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the unemployment rate like in Florida right now?"

**🤖 AI Agent:**
> Florida currently reports an unemployment rate of 2.9%, significantly below the 3.7% national average.

---

**👤 You:**
> "Identify which MSAs (Metros) have the lowest and highest rates."

**🤖 AI Agent:**
> Metros with the lowest unemployment include places like Fargo, ND (1.7%), while high-rate metros include El Centro, CA hovering near 15%.

---

**👤 You:**
> "How did New York perform post-pandemic on employment?"

**🤖 AI Agent:**
> New York struggled initially hitting double digits, but successfully cooled the unemployment readings down to near 4.3% presently, driven by tech and services rebounds.


## ❓ FAQ

**Q: Does it list ALL US Counties?**
Yes, LAUS captures more than 3,100 specific county data-series actively every month.

**Q: How to get a key?**
Go to data.bls.gov/registrationEngine. It's totally free.

**Q: Can it run with Jobs data?**
Yes, merging state LAUS data with national CES nonfarm data provides an excellent contrast for macro reports.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bls-local-laus-state-county-unemployment](https://vinkius.com/mcp/bls-local-laus-state-county-unemployment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BLS Local — LAUS State & County Unemployment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bls-local-laus-state-county-unemployment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BLS Local — LAUS State & County Unemployment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bls-local-laus-state-county-unemployment": {
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
