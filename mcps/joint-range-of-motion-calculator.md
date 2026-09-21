# Joint Range of Motion Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/joint-range-of-motion-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Quantifies mobility deficits by comparing measured joint movement against normative clinical data.

## Description
This MCP server provides clinical decision support for assessing joint mobility. It allows AI agents to retrieve standardized movement ranges using `get_normative_reference` and calculate specific clinical metrics like deficit and functional impact via `calculate_rom_metrics`. Clinicians can use `evaluate_mobility_status` to get a complete assessment of a patient's movement, or `get_joint_capabilities` to identify valid movement directions for a specific joint. It bridges the gap between raw physical measurements and actionable clinical insights.


## Available Tools (4)
- **evaluate_mobility_status**: Provides a summary assessment of a single measurement
- **get_joint_capabilities**: Lists all valid movements and directions available for a specific joint
- **get_normative_reference**: Retrieves the expected normal ROM for a specific joint and movement profile
- **calculate_rom_metrics**: Computes the comparison between measured movement and normative standards


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Joint Range of Motion Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Assess the mobility status for a 45-year-old male with a shoulder flexion angle of 140 degrees."

**🤖 AI Agent:**
> The shoulder flexion for a 45-year-old male is within the normal range. The measured 140 degrees is sufficient compared to the normative standard.

---

**👤 You:**
> "What are the valid movement directions for the knee joint?"

**🤖 AI Agent:**
> The valid movement directions for the knee are flexion and extension.

---

**👤 You:**
> "Calculate the ROM metrics for a knee extension of 160 degrees when the normal angle is 170 degrees and the target is 175 degrees."

**🤖 AI Agent:**
> The patient has achieved 94.1% of the normal range, with a deficit of 10 degrees. The functional impact is classified as Minimal.


## ❓ FAQ

**Q: How does the tool determine if a movement is normal?**
The tool uses `get_normative_reference` to fetch expected angles based on the patient's age, gender, and the specific joint and direction being measured.

**Q: Can I see all possible movements for a specific joint?**
Yes, you can use the `get_joint_capabilities` tool to list all valid movement directions supported for any given joint.

**Q: What kind of metrics are provided?**
By using `calculate_rom_metrics`, the tool provides the percentage of normal movement, the degree of deficit, and a qualitative functional impact assessment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/joint-range-of-motion-calculator](https://vinkius.com/en/ai-agent-connect/joint-range-of-motion-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Joint Range of Motion Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `joint-range-of-motion-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Joint Range of Motion Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "joint-range-of-motion-calculator": {
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
