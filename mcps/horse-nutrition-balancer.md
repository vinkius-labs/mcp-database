# Horse Nutrition Balancer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/horse-nutrition-balancer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate precise equine nutrient requirements and optimize rations using NRC standards.

## Description
This MCP server provides professional-grade equine nutrition tools. It allows AI agents to determine specific biological needs through `calculate_nutrient_requirements`, design balanced diets with `balance_ration`, and assess metabolic health risks using `analyze_metabolic_risk`. It uses National Research Council (NRC) guidelines to manage energy, protein, minerals, and NSC levels for horses in various physiological states, including growing, pregnant, or performance horses.


## Available Tools (3)
- **analyze_metabolic_risk**: Evaluates the risk of metabolic syndrome based on the proposed ration
- **balance_ration**: Calculates the ideal amount of forage and concentrate to meet the previously calculated requirements
- **calculate_nutrient_requirements**: Determines the specific biological nutrient needs for a horse based on its physical and physiological profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Horse Nutrition Balancer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the nutrient requirements for a 500kg horse, 5 years old, with moderate work level?"

**🤖 AI Agent:**
> The requirements for this horse are 18.5 Mcal/day of digestible energy, 450g of crude protein, and 12g of lysine.

---

**👤 You:**
> "Help me balance a ration for a 450kg pregnant mare using this forage analysis: { 'de': 1.8, 'cp': 10, 'nsc': 15, 'ca': 0.5, 'p': 0.3 } and 8kg of forage."

**🤖 AI Agent:**
> To meet the requirements for the pregnant mare, you should provide 8kg of forage and 2.4kg of concentrate.

---

**👤 You:**
> "Is this ration safe for a horse with high metabolic sensitivity?"

**🤖 AI Agent:**
> The risk score is 15, which is low. The NSC levels are within the safe range for this sensitivity profile.


## ❓ FAQ

**Q: How does the tool calculate nutrient needs?**
The `calculate_nutrient_requirements` tool uses NRC equine requirements to scale needs based on weight, age, work intensity, and reproductive status.

**Q: Can I check for metabolic risks?**
Yes, you can use `analyze_metabolic_risk` to evaluate the risk of metabolic syndrome based on the NSC levels in a proposed ration.

**Q: Does it handle performance horses?**
Yes, the system accounts for different work levels, including heavy activity for performance horses, to ensure adequate digestible energy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/horse-nutrition-balancer](https://vinkius.com/ai-agent-connect/horse-nutrition-balancer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Horse Nutrition Balancer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `horse-nutrition-balancer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Horse Nutrition Balancer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "horse-nutrition-balancer": {
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
