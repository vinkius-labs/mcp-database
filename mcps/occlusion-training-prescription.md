# Occlusion Training Prescription MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/occlusion-training-prescription)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Prescribe safe KAATSU-style BFR training protocols.

## Description
This MCP server provides specialized Blood Flow Restriction (BFR) training prescriptions using KAATSU-style principles. It allows AI agents to calculate safe occlusion pressures via `get_pressure_prescription`, recommend biomechanically appropriate exercises with `get_exercise_recommendation`, design specific training volumes using `get_repetition_scheme`, and provide real-time safety monitoring through `get_safety_protocol`.


## Available Tools (4)
- **get_exercise_recommendation**: Selects appropriate exercises based on the target muscle group and training goal
- **get_pressure_prescription**: Determines the safe occlusion pressure for a specific user
- **get_repetition_scheme**: Generates the specific set and repetition structure for a session
- **get_safety_protocol**: Provides a real-time monitoring checklist for the trainee


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Occlusion Training Prescription** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am a novice trainee looking to build muscle in my thighs. What is my pressure and what exercises should I do?"

**🤖 AI Agent:**
> For a novice training thighs for hypertrophy, your recommended pressure is 40% of physiological baseline. You should perform leg extensions and goblet squats.

---

**👤 You:**
> "Give me a strength training rep scheme for an advanced user."

**🤖 AI Agent:**
> For an advanced user focusing on strength, the protocol is 4 sets of 6 repetitions with a 90-second rest interval.

---

**👤 You:**
> "What safety precautions should I follow as a novice?"

**🤖 AI Agent:**
> As a novice, you must monitor for limb color changes, numbness, or intense pain. Stop immediately if you feel any tingling or significant discomfort.


## ❓ FAQ

**Q: What is BFR training?**
Blood Flow Restriction (BFR) training involves applying controlled pressure to limbs to restrict venous return, allowing for muscle growth using lower mechanical loads.

**Q: How is the pressure determined?**
The `get_pressure_prescription` tool calculates safe pressure based on the target muscle group and the user's experience level.

**Q: Can I use this for strength training?**
Yes, you can specify 'strength' as the training goal to receive appropriate exercise and repetition recommendations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/occlusion-training-prescription](https://vinkius.com/en/ai-agent-connect/occlusion-training-prescription)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Occlusion Training Prescription** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `occlusion-training-prescription` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Occlusion Training Prescription** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "occlusion-training-prescription": {
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
