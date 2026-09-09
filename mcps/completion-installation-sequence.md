# Completion Installation Sequence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/completion-installation-sequence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Technical planning tool for oil and gas well completion workflows.

## Description
This MCP server provides specialized tools for oil and gas operations to plan well completion sequences. It allows engineers to generate chronological installation timelines using `plan_sequence_timeline`, calculate fluid requirements with `calculate_displacement_needs`, determine safe velocities via `optimize_running_speeds`, and ensure safety compliance through `validate_installation_readiness`.


## Available Tools (4)
- **calculate_displacement_needs**: Determines how much fluid is required to move equipment or fill the wellbore during specific phases
- **optimize_running_speeds**: Determines the safest and most efficient velocity for lowering/raising equipment
- **plan_sequence_timeline**: Generates the complete chronological list of installation steps and their estimated durations
- **validate_installation_readiness**: Checks if the provided plan meets all mandatory safety and testing requirements before execution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Completion Installation Sequence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a timeline for a completion design with these specs."

**🤖 AI Agent:**
> The installation sequence is complete: 1. Run tubing to 5000ft, 2. Set packer at 5100ft, 3. Pressure test seal.

---

**👤 You:**
> "What is the required fluid volume for this equipment at 3000ft?"

**🤖 AI Agent:**
> The required displacement volume at 3000ft is 450 barrels of drilling mud.

---

**👤 You:**
> "What is the recommended running speed for this string?"

**🤖 AI Agent:**
> The recommended lowering speed is 15 ft/min to maintain wellbore stability.


## ❓ FAQ

**Q: How do I generate a full installation timeline?**
You can use the `plan_sequence_timeline` tool by providing the completion design, well conditions, and equipment specifications.

**Q: Can I check if my plan meets safety requirements?**
Yes, the `validate_installation_readiness` tool checks your plan against mandatory testing and safety requirements.

**Q: How is displacement volume calculated?**
The `calculate_displacement_needs` tool calculates volume based on the annular space between the equipment and the wellbore.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/completion-installation-sequence](https://vinkius.com/ai-agent-connect/completion-installation-sequence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Completion Installation Sequence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `completion-installation-sequence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Completion Installation Sequence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "completion-installation-sequence": {
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
