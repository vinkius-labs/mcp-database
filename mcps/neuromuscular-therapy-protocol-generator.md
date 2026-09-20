# Neuromuscular Therapy Protocol Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/neuromuscular-therapy-protocol-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Generates clinical NMT treatment sequences, pressure regimes, and stretching protocols.

## Description
This MCP server provides a complete suite of tools for Neuromuscular Therapy (NMT) professionals. It converts clinical data like postural distortions and trigger point maps into actionable therapeutic plans. Use `generate_treatment_plan` to create ordered sequences, `calculate_pressure_regime` to determine ischemic hold durations, `design_stretching_protocol` for post-manipulation movements, and `analyze_clinical_stability` to ensure treatment safety.


## Available Tools (4)
- **analyze_clinical_stability**: Evaluates if the proposed protocol is safe and logical based on the relationship between posture and biomechanics
- **calculate_pressure_regime**: Determines the specific type of pressure and how long to hold it for identified trigger points
- **design_stretching_protocol**: Creates a series of corrective stretches to be performed following the manual pressure application
- **generate_treatment_plan**: Generates a complete, ordered NMT treatment sequence based on a patient's clinical profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Neuromuscular Therapy Protocol Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a treatment plan for a patient with anterior pelvic tilt and hip muscle spasticity."

**🤖 AI Agent:**
> The treatment sequence will prioritize stabilizing the pelvic region before addressing deep tissue tension in the hip flexors.

---

**👤 You:**
> "Calculate the pressure regime for a trigger point in the trapezius with a severity of 8."

**🤖 AI Agent:**
> For a severity of 8, the system recommends a sustained compression technique with an ischemic hold duration of 45 seconds.

---

**👤 You:**
> "Design a stretching protocol for someone with scapular winging."

**🤖 AI Agent:**
> The protocol includes serratus anterior activation and pectoral stretching to correct the scapular position.


## ❓ FAQ

**Q: How do I generate a full treatment plan?**
You can use the `generate_treatment_plan` tool by providing the patient's postural distortions, biomechanical dysfunctions, and a trigger point map.

**Q: Can I check if a protocol is safe?**
Yes, the `analyze_clinical_stability` tool evaluates the relationship between posture and biomechanics to ensure the sequence is safe.

**Q: How are stretching protocols determined?**
The `design_stretching_protocol` tool creates corrective stretches specifically targeting the muscles identified in the patient's biomechanical data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/neuromuscular-therapy-protocol-generator](https://vinkius.com/en/ai-agent-connect/neuromuscular-therapy-protocol-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Neuromuscular Therapy Protocol Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `neuromuscular-therapy-protocol-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Neuromuscular Therapy Protocol Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "neuromuscular-therapy-protocol-generator": {
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
