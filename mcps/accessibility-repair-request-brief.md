# Accessibility Repair Request Brief MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessibility-repair-request-brief)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [property-management](../categories/property-management.md)

Generate professional accessibility repair documentation, provider scope questions, and implementation timelines.

## Description
This MCP server provides a suite of tools to transform accessibility barriers into structured, professional documentation. It helps stakeholders like tenants and landlords generate factual request briefs, technical questions for contractors via `provider_scope_interrogator`, and project timelines using `timeline_estimator`. The `documentation_packer` then bundles these into a complete package for submission. It is designed to bridge the gap between physical access needs and professional repair implementation.


## Available Tools (4)
- **timeline_estimator**: Projects the stages and duration of the repair project
- **documentation_packer**: Compiles the final formal package for submission
- **provider_scope_interrogator**: Generates a list of technical questions to ask contractors/service providers
- **request_brief_generator**: Generates a factual, professional summary of the accessibility issue for stakeholders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessibility Repair Request Brief** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need a summary for a landlord. There is a 5cm step at the front door, the layout is a narrow hallway, and the recommendation is to install a modular ramp. The budget is $500."

**🤖 AI Agent:**
> Request Summary: Installation of a modular ramp at the primary entrance to resolve a 5cm step barrier. Stakeholder Authority: Tenant. Budget Status: Within allocated funds.

---

**👤 You:**
> "Generate technical questions for a contractor. The barrier is a narrow doorway (70cm), the layout is a standard residential corridor, and the recommendation is to widen the door to 90cm."

**🤖 AI Agent:**
> 1. Given the narrow hallway, how will the installation of the widened door frame impact the structural clearance of the corridor? 2. What materials are required to maintain the existing wall finish while widening the opening?

---

**👤 You:**
> "Estimate a timeline for widening a doorway with a budget of $2000."

**🤖 AI Agent:**
> Phase 1: Site preparation and debris removal (2 days). Phase 2: Structural widening and frame installation (3 days). Phase 3: Finishing and cleanup (2 days). Total estimated duration: 7 days.


## ❓ FAQ

**Q: Does this tool provide medical assessments?**
No. This tool is strictly for generating physical repair documentation and does not provide any medical or health assessments.

**Q: How can I use the timeline estimator?**
You can use the `timeline_estimator` by providing the professional recommendations and the allocated budget to project the repair phases.

**Q: Can I generate questions for my contractor?**
Yes, the `provider_scope_interrogator` generates technical questions specifically tailored to the physical layout and the recommended solution.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessibility-repair-request-brief](https://vinkius.com/en/ai-agent-connect/accessibility-repair-request-brief)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessibility Repair Request Brief** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessibility-repair-request-brief` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessibility Repair Request Brief** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessibility-repair-request-brief": {
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
