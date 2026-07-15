# SBOM Dependency Risk Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sbom-dependency-risk-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Analyze SBOM files to quantify supply chain risk through dependency structure, package staleness, and vulnerability exposure.

## Description
The SBOM Dependency Risk Scorer is an analytical engine designed to evaluate the security and maintenance health of software ecosystems. By processing Software Bill of Materials (SPDX/CycloneDX) files, it quantifies risk across three critical vectors: structural complexity, maintenance decay, and known vulnerability exposure. Use `analyze_dependency_structure` to assess dependency depth, `evaluate_package_stalness` to identify outdated components, `tally_vulnerability_exposure` to count CVEs, and `calculate_composite_risk_score` to generate a single, actionable risk rating.


## Available Tools (4)
- **analyze_dependency_structure**: Analyzes the dependency tree structure of an SBOM
- **calculate_composite_risk_score**: Calculates the final security risk score
- **evaluate_package_stalness**: Evaluates how outdated packages are based on release dates
- **tally_vulnerability_exposure**: Counts known vulnerabilities in the SBOM


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SBOM Dependency Risk Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How complex is my dependency tree in this SBOM?"

**🤖 AI Agent:**
> The dependency tree contains 45 total dependencies, with a direct-to-transitive ratio of 0.22, indicating significant nested complexity.

---

**👤 You:**
> "Are there any high-severity vulnerabilities in my project?"

**🤖 AI Agent:**
> The analysis found 3 high-severity vulnerabilities and 12 low-severity vulnerabilities within the provided SBOM content.

---

**👤 You:**
> "What is my overall supply chain risk score?"

**🤖 AI Agent:**
> Your project has a Risk Level of High, driven primarily by high vulnerability density and significant package staleness.


## ❓ FAQ

**Q: What types of SBOM formats are supported?**
The engine supports both SPDX and CycloneDX formats for analyzing dependency structures.

**Q: How is the final risk score calculated?**
The `calculate_composite_risk_score` tool aggregates metrics from structural complexity, package staleness, and vulnerability counts to produce a normalized risk level.

**Q: Can I use this to find outdated packages?**
Yes, by using the `evaluate_package_stalness` tool with a reference date, you can identify components that have not been updated recently.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sbom-dependency-risk-scorer](https://vinkius.com/mcp/sbom-dependency-risk-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SBOM Dependency Risk Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sbom-dependency-risk-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SBOM Dependency Risk Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sbom-dependency-risk-scorer": {
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
