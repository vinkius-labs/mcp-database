# Steel Fabrication Tolerance Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/steel-fabrication-tolerance-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate precise fabrication tolerances for steel members using AISC or EN 1090 standards.

## Description
This MCP server provides essential engineering tools for structural steel fabrication. It allows AI agents to determine allowable deviations for steel components based on international regulatory standards. Use `calculate_member_tolerances` to find specific limits for length, straightness, and hole positioning. You can also use `get_code_guidelines` to understand the philosophy of AISC or EN 1090, or `validate_component_fit` to check if a manufactured part meets its required specifications.


## Available Tools (4)
- **lookup_section_defaults**: Provides the default base dimensions and scaling factors for common steel shapes
- **calculate_member_tolerances**: Provides the core set of acceptable fabrication tolerances for a specific steel component
- **get_code_guidelines**: Retrieves the high-level tolerance philosophy and general rules for a specific regulatory code
- **validate_component_fit**: Checks if a manufactured component's measured deviations are within the acceptable limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Steel Fabrication Tolerance Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the tolerances for a 6m I-Beam, primary structural, using AISC for a bolted connection?"

**🤖 AI Agent:**
> The allowable tolerances for your 6m I-Beam are a length deviation of 2.5mm, a straightness deviation of 4.0mm, and a hole position deviation of 1.5mm.

---

**👤 You:**
> "Get the general philosophy for the EN 1090 standard."

**🤖 AI Agent:**
> The EN 1090 standard focuses on execution classes to ensure structural integrity across European construction projects, primarily using metric units.

---

**👤 You:**
> "Is a component with 3mm straightness deviation acceptable if the limit is 2mm?"

**🤖 AI Agent:**
> No, the component is not acceptable because the measured straightness exceeds the target tolerance.


## ❓ FAQ

**Q: Which standards are supported?**
The server supports AISC (American Institute of Steel Construction) and EN 1090 (Eurocode) standards.

**Q: How do I check if a part is within tolerance?**
You can use the `validate_component_fit` tool by providing the target tolerances and the actual measured values.

**Q: Does it handle bolted connections?**
Yes, for bolted connections, the tool provides a specific `holePositionTolerance` to ensure assembly alignment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/steel-fabrication-tolerance-calculator](https://vinkius.com/ai-agent-connect/steel-fabrication-tolerance-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Steel Fabrication Tolerance Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `steel-fabrication-tolerance-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Steel Fabrication Tolerance Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "steel-fabrication-tolerance-calculator": {
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
