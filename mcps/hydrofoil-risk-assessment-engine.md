# Hydrofoil Risk Assessment Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/hydrofoil-risk-assessment-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [hydrodynamics](../categories/hydrodynamics.md)

Predict and mitigate ventilation and cavitation risks for hydrofoil vessels.

## Description
This MCP server provides high-fidelity risk assessment for hydrofoil operations. It allows AI agents to monitor and predict critical stability issues like ventilation and cavitation. Using tools like `calculate_ventilation_risk` and `check_cavitation_limits`, agents can determine safe speed thresholds, assess stability during maneuvers with `analyze_maneuver_stability`, and retrieve performance data via `get_design_performance_envelope`. This ensures safe vessel operation by providing actionable recovery instructions based on real-time environmental and design data.


## Available Tools (4)
- **analyze_maneuver_stability**: Assesses how a planned change in direction (turn) will affect the current stability envelope
- **calculate_ventilation_risk**: Determines the immediate risk level of air being sucked into the hydrofoil
- **check_cavitation_limits**: Evaluates if the foil is operating in a regime where vapor bubbles will form on the foil surface
- **get_design_performance_envelope**: Retrieves the theoretical safety limits for a specific wing geometry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hydrofoil Risk Assessment Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the ventilation risk for a foil traveling at 15 m/s with 40% mast immersion and a 50m turn radius?"

**🤖 AI Agent:**
> The ventilation risk score is 7. Your maximum safe speed is 12 m/s. Recommended action: Reduce speed immediately.

---

**👤 You:**
> "Is my wing design 'Alpha-V1' safe at 20 m/s with 80% immersion?"

**🤖 AI Agent:**
> The cavitation risk score for 'Alpha-V1' at 20 m/s is 2. The safe operating limit is 25 m/s. You are operating safely.

---

**👤 You:**
> "How will a turn with a 20m radius affect my stability at 10 m/s and 50% immersion?"

**🤖 AI Agent:**
> The stability impact is Critical. The recommended maximum radius to maintain stability at this speed is 45m.


## ❓ FAQ

**Q: How does the engine calculate ventilation risk?**
The engine uses `calculate_ventilation_risk` to evaluate foil speed, mast immersion, turn radius, surface chop, and mast angle to produce a risk score and safe speed threshold.

**Q: Can I check if my specific wing design is safe at high speeds?**
Yes, you can use `get_design_performance_envelope` to find the max design speed and `check_cavitation_limits` to evaluate cavitation risk for a specific wing design.

**Q: What happens if the risk score is high?**
The tool provides a specific `recoveryAction`, such as reducing speed or increasing immersion, to return the vessel to a safe operating envelope.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/hydrofoil-risk-assessment-engine](https://vinkius.com/en/ai-agent-connect/hydrofoil-risk-assessment-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hydrofoil Risk Assessment Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hydrofoil-risk-assessment-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hydrofoil Risk Assessment Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hydrofoil-risk-assessment-engine": {
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
