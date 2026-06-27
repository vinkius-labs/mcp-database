# US Seismic Zone Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-seismic-zone-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Identify Seismic Design Categories and structural detailing requirements based on US regional seismic data.

## Description
The US Seismic Zone Checker provides critical earthquake risk information for engineers and builders. By using tools like `verify_location_validity`, `lookup_seismic_info`, and `retrieve_structural_requirements`, users can determine the Seismic Design Category (SDC) for specific US counties. The tool retrieves spectral acceleration values ($S_s$ and $S_1$) and provides mandatory structural detailing instructions as defined by the International Building Code (IBC). This ensures that construction projects meet the necessary seismic safety standards based on regional earthquake intensity.


## Available Tools (3)
- **lookup_seismic_info**: Retrieve specific seismic parameters and design category
- **retrieve_structural_requirements**: Provide mandatory structural detailing rules for a specific SDC
- **verify_location_validity**: Check if a provided State and County combination exists


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Seismic Zone Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is Los Angeles, California a valid location in your database?"

**🤖 AI Agent:**
> Yes, Los Angeles, California is a valid location in the seismic database.

---

**👤 You:**
> "What is the Seismic Design Category for San Francisco, CA?"

**🤖 AI Agent:**
> The Seismic Design Category for San Francisco, CA is D.

---

**👤 You:**
> "What are the structural requirements for SDC E?"

**🤖 AI Agent:**
> For SDC E, the requirements include intensive reinforcement of concrete members and specific masonry joint detailing to withstand high seismic forces.


## ❓ FAQ

**Q: How can I check if a specific county is covered?**
You can use the `verify_location_validity` tool by providing the state and county name to see if it exists in our seismic database.

**Q: What information does the lookup tool provide?**
The `lookup_seismic_info` tool returns the Seismic Design Category (SDC), as well as the Short-Period ($S_s$) and One-Second ($S_1$) spectral acceleration values.

**Q: Does this tool provide structural engineering rules?**
Yes, by using `retrieve_structural_requirements` with a specific SDC (A-F), you can get the mandatory detailing instructions required by the IBC.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-seismic-zone-checker](https://vinkius.com/mcp/us-seismic-zone-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Seismic Zone Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-seismic-zone-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Seismic Zone Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-seismic-zone-checker": {
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
