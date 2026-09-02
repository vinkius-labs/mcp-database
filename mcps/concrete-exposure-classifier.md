# Concrete Exposure Classifier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-exposure-classifier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Determines concrete exposure classification and required material specifications.

## Description
This MCP server provides engineering tools to classify concrete exposure based on environmental stressors like chloride levels, freeze-thaw cycles, and carbonation risk. It uses `get_exposure_classification` to identify required material properties such as minimum concrete grade, maximum w/c ratio, and minimum cover. Engineers can also use `validate_material_compliance` to verify mix designs, `check_freeze_thaw_mitigation` for air-entrainment needs, and `calculate_carbonation_depth_risk` to estimate corrosion onset.


## Available Tools (4)
- **calculate_carbonation_depth_risk**: Estimate the risk level of carbonation based on environmental factors
- **check_freeze_thaw_mitigation**: Determine specific requirements for air-entrainment or density when freeze-thaw cycles are a primary concern
- **get_exposure_classification**: Identify the specific exposure class and required material specifications for a given set of environmental conditions
- **validate_material_compliance**: Verify if a proposed concrete mix design meets the requirements of a specific exposure class


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Exposure Classifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the concrete requirements for a marine environment with high chloride levels and a 50-year design life?"

**🤖 AI Agent:**
> For a marine environment with high chloride levels and a 50-year design life, the required minimum concrete grade is 40 MPa, the maximum w/c ratio is 0.40, and the minimum reinforcement cover is 50 mm.

---

**👤 You:**
> "Is a concrete mix with a grade of 30 MPa, w/c ratio of 0.5, and 30mm cover compliant for a moderate exposure class?"

**🤖 AI Agent:**
> No, the proposed mix is not compliant. The w/c ratio of 0.5 exceeds the maximum allowed for this class, and the 30mm cover is below the required minimum.

---

**👤 You:**
> "What is the carbonation risk for concrete with 0.7 humidity and 0.2 porosity?"

**🤖 AI Agent:**
> The carbonation risk is high. The estimated years to corrosion onset is 15 years, and a minimum cover of 45 mm is recommended.


## ❓ FAQ

**Q: How do I know if my concrete mix is compliant?**
You can use the `validate_material_compliance` tool by providing the target exposure class, the proposed grade, w/c ratio, and reinforcement cover.

**Q: Can this tool account for protective coatings?**
Yes, when using `get_exposure_classification`, you can specify if protective measures are being used to potentially relax certain requirements.

**Q: What standards does the classification follow?**
The system reconciles requirements based on international standards including ACI, EN, and AS.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-exposure-classifier](https://vinkius.com/ai-agent-connect/concrete-exposure-classifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Exposure Classifier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-exposure-classifier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Exposure Classifier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-exposure-classifier": {
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
