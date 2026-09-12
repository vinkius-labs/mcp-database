# Lockout/Tagout Procedure Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/lockouttagout-procedure-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [compliance](../categories/compliance.md)

Generates OSHA-compliant lockout/tagout (LOTO) procedures for industrial equipment.

## Description
This MCP server provides a complete safety suite for generating standardized lockout/tagout (LOTO) procedures. It connects AI agents to critical safety logic to ensure worker protection during maintenance. Using tools like `get_isolation_points` to identify energy control locations, `get_verification_steps` to confirm zero energy states, and `calculate_group_lockout_needs` for multi-worker coordination, it ensures every procedure follows OSHA standards. The `generate_loto_procedure` tool compiles all data into a single, cohesive safety document covering identification, isolation, verification, and shift handovers.


## Available Tools (4)
- **generate_loto_procedure**: Compiles all individual safety components into a single, cohesive, and compliant LOTO document
- **get_isolation_points**: Identifies the specific physical locations where energy must be controlled
- **get_verification_steps**: Provides the specific physical actions required to confirm zero energy state
- **calculate_group_lockout_needs**: Determines the requirements for a coordinated lockout when multiple personnel are involved


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lockout/Tagout Procedure Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a LOTO procedure for a Conveyor Belt with electrical and pneumatic energy sources for 3 workers."

**🤖 AI Agent:**
> Procedure ID: LOTO-CB-992. Equipment: Conveyor Belt. Isolation Steps: 1. Turn off main electrical disconnect. 2. Close pneumatic supply valve. Verification Steps: 1. Attempt to restart via control panel. 2. Check pressure gauges for zero pneumatic pressure. Group Safety: 3 locks required for 3 workers.

---

**👤 You:**
> "What are the isolation points for a Hydraulic Press with hydraulic energy?"

**🤖 AI Agent:**
> The isolation point for the Hydraulic Press is the main hydraulic fluid supply valve located at the primary manifold.

---

**👤 You:**
> "How many locks are needed for a 5-person maintenance crew?"

**🤖 AI Agent:**
> A total of 5 locks are required for a 5-person maintenance crew to ensure individual protection.


## ❓ FAQ

**Q: Does this tool comply with OSHA standards?**
Yes, the procedures are designed to follow OSHA LOTO regulations to ensure a zero energy state is achieved and verified.

**Q: How does it handle multiple workers?**
It uses `calculate_group_lockout_needs` to determine the required number of locks and specific handover protocols for multi-worker or multi-shift scenarios.

**Q: Can I use this for different types of machinery?**
Yes, the system supports various equipment types and energy sources including electrical, pneumatic, and hydraulic energy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/lockouttagout-procedure-generator](https://vinkius.com/en/ai-agent-connect/lockouttagout-procedure-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lockout/Tagout Procedure Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lockouttagout-procedure-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lockout/Tagout Procedure Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lockouttagout-procedure-generator": {
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
