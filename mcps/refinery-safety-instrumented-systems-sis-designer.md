# Refinery Safety Instrumented Systems (SIS) Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/refinery-safety-instrumented-systems-sis-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design and validate safety instrumented systems (SIS) following IEC 61511 standards.

## Description
This MCP server provides specialized tools for refinery safety engineering. It allows AI agents to perform critical safety calculations including `calculate_sil_requirement` to determine target risk reduction, `evaluate_voting_logic` for hardware architecture, `calculate_proof_test_interval` for maintenance scheduling, and `analyze_sif_reliability` to validate if a design meets its safety targets. All calculations adhere to IEC 61511 methodologies for Safety Instrumented Functions (SIF).


## Available Tools (4)
- **calculate_proof_test_interval**: Determine the safe interval between mandatory system tests
- **calculate_sil_requirement**: Determine the target SIL level required for a specific process hazard
- **evaluate_voting_logic**: Determine the appropriate hardware architecture (voting) for a SIF
- **analyze_sif_reliability**: Assess whether a proposed SIF design meets the necessary safety targets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Refinery Safety Instrumented Systems (SIS) Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the required SIL if the risk reduction factor needed is 150 and the current risk is 0.1?"

**🤖 AI Agent:**
> The required target SIL is SIL 2.

---

**👤 You:**
> "Calculate the proof test interval for a configuration with a PFD of 0.001 and a component failure rate of 0.0001."

**🤖 AI Agent:**
> The recommended proof test interval is 1000 days, with a maximum safe interval of 1200 days.

---

**👤 You:**
> "Is a 1oo2 configuration with two sensors having a failure rate of 0.002 compliant for SIL 2?"

**🤖 AI Agent:**
> Yes, the design is compliant with the target SIL 2.


## ❓ FAQ

**Q: Does this tool follow IEC 61511 standards?**
Yes, all calculations for SIL, voting logic, and proof test intervals are based on IEC 61511 methodologies.

**Q: How can I verify if my SIF design is compliant?**
You can use the `analyze_sif_reliability` tool to assess whether your proposed design meets the required target SIL level.

**Q: Can I calculate the required risk reduction?**
Yes, the `calculate_sil_requirement` tool determines the target SIL level based on the risk reduction factor and current risk levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/refinery-safety-instrumented-systems-sis-designer](https://vinkius.com/en/ai-agent-connect/refinery-safety-instrumented-systems-sis-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Refinery Safety Instrumented Systems (SIS) Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `refinery-safety-instrumented-systems-sis-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Refinery Safety Instrumented Systems (SIS) Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "refinery-safety-instrumented-systems-sis-designer": {
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
