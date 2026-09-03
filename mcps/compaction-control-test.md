# Compaction Control Test MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/compaction-control-test)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Analyzes soil compaction quality by comparing field test results against laboratory standards.

## Description
This MCP server provides specialized engineering analysis for civil engineering projects. It connects AI agents to critical soil stability data, allowing for the evaluation of field density tests against laboratory-determined Maximum Dry Density (MDD). Using tools like `analyze_compaction_status`, agents can determine if a soil layer meets project specifications, assess moisture suitability via `check_moisture_suitability`, and retrieve specific remediation steps through `get_rework_protocol`. It is designed to handle various soil types, including clay, silt, and sand, while accounting for layer thickness and moisture deviations.


## Available Tools (4)
- **analyze_compaction_status**: Evaluates if a specific test result meets the project's engineering requirements
- **check_moisture_suitability**: Determines if the current moisture level is within an acceptable range for the specific soil type
- **get_rework_protocol**: Provides detailed instructions on how to fix a failed compaction test
- **validate_test_parameters**: Ensures all input data for a compaction test is physically possible and within reasonable engineering bounds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Compaction Control Test** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this compaction test: wet density 1950 kg/m³, moisture 12%, MDD 1900 kg/m³, OMC 11%, spec 95%, soil is clay, layer thickness 0.3m."

**🤖 AI Agent:**
> The relative compaction is 102.6% and the dry density is 1741.07 kg/m³. The test meets the specification requirement.

---

**👤 You:**
> "Is a moisture content of 15% suitable for a clay soil with an OMC of 11%?"

**🤖 AI Agent:**
> No, the moisture is too wet for this clay soil.

---

**👤 You:**
> "What should I do if my compaction test failed due to low density in a 0.5m sand layer?"

**🤖 AI Agent:**
> You should increase the number of passes with a vibratory roller to achieve the required density.


## ❓ FAQ

**Q: How does the tool determine if a compaction test passed?**
The `analyze_compaction_status` tool calculates the relative compaction by comparing the field dry density to the laboratory Maximum Dry Density. If this percentage meets or exceeds the project's specification requirement, the test is marked as passing.

**Q: Can I get remediation steps for a failed test?**
Yes. If a test fails, you can use `get_rework_protocol` to receive specific physical instructions, equipment suggestions, and the expected outcome to correct the soil density or moisture levels.

**Q: Does the tool account for different soil types?**
Yes, the analysis considers whether the soil is clay, silt, or sand. This is critical because cohesive soils like clay have much narrower moisture tolerances than granular soils like sand.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/compaction-control-test](https://vinkius.com/ai-agent-connect/compaction-control-test)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Compaction Control Test** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `compaction-control-test` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Compaction Control Test** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "compaction-control-test": {
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
