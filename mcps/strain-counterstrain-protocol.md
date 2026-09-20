# Strain-Counterstrain Protocol MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/strain-counterstrain-protocol)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Generates standardized neuromuscular treatment protocols using Jones Counterstrain methodology.

## Description
This MCP server provides clinical decision support for practitioners using the Counterstrain (Jones) technique. It allows AI agents to calculate precise positions of comfort, determine optimal hold durations, and plan re-assessment strategies based on tender point locations and patient data. Use `generate_protocol` to create a full treatment plan, `validate_poc_viability` to check anatomical logic, `calculate_hold_parameters` for timing, and `get_reassessment_strategy` for post-treatment evaluation.


## Available Tools (4)
- **calculate_hold_parameters**: Calculates the precise duration and frequency of monitoring required for the hold phase
- **generate_protocol**: Generates a complete, step-by-step treatment protocol for a specific tender point
- **get_reassessment_strategy**: Determines how the practitioner should re-evaluate the patient after the treatment hold
- **validate_poc_viability**: Checks if a proposed Position of Comfort is anatomically logical


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Strain-Counterstrain Protocol** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a treatment protocol for a tender point at the right trapezius, associated with the cervical spine, with a comfort level of 8."

**🤖 AI Agent:**
> Protocol ID: CS-TRAP-001. Tender Point: Right Trapezius. Associated Joint: Cervical Spine. Position of Comfort: Lateral flexion to the left with slight rotation. Hold Duration: 90 seconds. Monitoring: Observe for muscle spindle relaxation. Re-assessment: Palpation comparison immediately after the hold.

---

**👤 You:**
> "Is a flexion/rotation position viable for a tender point at the left iliopsoas?"

**🤖 AI Agent:**
> The proposed position is viable for the iliopsoas tender point to reduce muscle spindle tension.

---

**👤 You:**
> "What should I do after a 90-second hold if the patient stayed in position?"

**🤖 AI Agent:**
> Perform a palpation comparison to check for reduced sensitivity at the tender point to verify the neutralization of the dysfunction.


## ❓ FAQ

**Q: How do I generate a full treatment plan?**
You can use the `generate_protocol` tool by providing the tender point location, the associated joint, and the client's comfort level.

**Q: Can I verify if a position is correct for a specific tender point?**
Yes, use the `validate_poc_viability` tool to check if a proposed position of comfort is anatomically logical for the given tender point and joint.

**Q: How is the hold duration determined?**
The duration is calculated using `calculate_hold_parameters`, which takes into account the intensity of the dysfunction and the patient's age.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/strain-counterstrain-protocol](https://vinkius.com/en/ai-agent-connect/strain-counterstrain-protocol)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Strain-Counterstrain Protocol** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `strain-counterstrain-protocol` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Strain-Counterstrain Protocol** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "strain-counterstrain-protocol": {
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
