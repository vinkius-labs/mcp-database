# Garden Hose Reach MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/garden-hose-reach)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Calculate hose reach, coverage, and capacity for gardening tasks.

## Description
This MCP server provides essential tools for managing garden hose usage. Use `check_reach` to determine if your hose can reach a target distance while accounting for obstacles, or `calculate_coverage_radius` to find the total area you can water. You can also use `validate_hose_capacity` to check hose categories or `compare_hose_sets` to pick the best hose from your collection for a specific job.


## Available Tools (4)
- **calculate_coverage_radius**: Calculates the maximum area a hose can cover if it were used to sweep a circular area around the water source
- **check_reach**: Determines if a specific hose can reach a target distance and calculates the excess or shortage
- **compare_hose_sets**: Compares multiple hoses to find which one provides the maximum remaining reach for a specific task
- **validate_hose_capacity**: Verifies if a hose length is within standard commercial manufacturing limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Garden Hose Reach** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can a 50ft hose reach a flower bed 40ft away if there are some bushes in the way (obstacle factor 1.2)?"

**🤖 AI Agent:**
> No, the hose is too short. With an obstacle factor of 1.2, the required distance is 48ft, leaving only 2ft of reach, but the calculation shows a deficit if the path is more complex.

---

**👤 You:**
> "What is the coverage area for a 25ft hose with a clear path?"

**🤖 AI Agent:**
> A 25ft hose with a clear path covers an area of approximately 1963.5 square feet.

---

**👤 You:**
> "Which is better for a 30ft distance: a 25ft hose or a 50ft hose?"

**🤖 AI Agent:**
> The 50ft hose is the best choice, providing 20ft of remaining reach.


## ❓ FAQ

**Q: How does the obstacle factor work?**
The obstacle factor increases the required distance to account for non-linear paths around bushes or fences. A factor of 1.0 represents a perfectly straight line.

**Q: Can I compare multiple hoses at once?**
Yes, you can use the `compare_hose_sets` tool to evaluate a list of available hose lengths against a target distance.

**Q: What is the difference between remaining reach and deficit?**
Remaining reach is the extra length available after reaching the target. A deficit occurs when the hose is too short to reach the destination.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/garden-hose-reach](https://vinkius.com/en/ai-agent-connect/garden-hose-reach)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Garden Hose Reach** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `garden-hose-reach` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Garden Hose Reach** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "garden-hose-reach": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
