# Rock Mass Characterization MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/rock-mass-characterization)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Quantify rock mass quality using RMR, Q-system, and GSI classification methods.

## Description
This MCP server provides essential tools for mining and civil engineering professionals to quantify rock mass mechanical quality. It implements industry-standard classification systems including RMR, the Q-system, and the Geological Strength Index (GSI). Engineers can use `get_rmr_classification` to determine support needs, `get_q_index` for tunnel-specific design, and `get_gsi_properties` to estimate strength reduction. Additionally, `analyze_structural_domain` evaluates stability risks caused by anisotropy and joint orientation within specific geological zones.


## Available Tools (4)
- **analyze_structural_domain**: Evaluates how anisotropy and orientation impact the overall stability of a specific structural domain
- **get_gsi_properties**: Estimates rock mass strength characteristics using the Geological Strength Index
- **get_q_index**: Calculates the Q-system Quality Index for tunnel-specific support design
- **get_rmr_classification**: Calculates the Rock Mass Rating (RMR) to determine rock mass quality and basic support needs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rock Mass Characterization** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the RMR for a rock mass with high strength, 75% RQD, 200mm joint spacing, very rough joints, and completely dry conditions with no orientation penalty."

**🤖 AI Agent:**
> The Rock Mass Rating (RMR) is 72, which falls into the 'Good Rock' quality class.

---

**👤 You:**
> "What is the Q-index if RQD is 60, there are 3 joint sets, joint alteration is 1, and the stress reduction factor is 2.5?"

**🤖 AI Agent:**
> The Q-system Quality Index is 4.8, suggesting a specific excavation support category.

---

**👤 You:**
> "Estimate the strength reduction for a massive rock structure with unweathered joint surfaces using GSI."

**🤖 AI Agent:**
> The GSI score is 90, resulting in a very low estimated strength reduction factor.


## ❓ FAQ

**Q: What classification systems are supported?**
The server supports Rock Mass Rating (RMR), the Q-system (Quality Index), and the Geological Strength Index (GSI).

**Q: Can I analyze specific geological zones?**
Yes, you can use `analyze_structural_domain` to evaluate stability risks and anisotropy impacts for a specific domain ID.

**Q: How is the RMR calculated?**
The `get_rmr_classification` tool calculates the score based on rock strength, RQD, joint spacing, condition, groundwater, and orientation adjustments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/rock-mass-characterization](https://vinkius.com/en/ai-agent-connect/rock-mass-characterization)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rock Mass Characterization** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rock-mass-characterization` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rock Mass Characterization** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rock-mass-characterization": {
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
