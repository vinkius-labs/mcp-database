# Hair Dye Formulation Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/hair-dye-formulation-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Calculate precise color tube counts and developer volumes for professional hair coloring.

## Description
This MCP server provides professional hair colorists with deterministic tools to calculate exact chemical formulations. Use `calculate_color_formulation` to determine the required number of 60ml color tubes and developer volume based on hair length, thickness, and application type. For lightening procedures, `calculate_bleach_mixture` provides the exact ratio of bleach powder to developer. Additionally, `get_strand_test_recommendation` offers safety guidance to prevent over-processing based on the level gap between current and target hair colors.


## Available Tools (3)
- **calculate_bleach_mixture**: Calculates the specific volumes of bleach powder and developer for lightening procedures
- **calculate_color_formulation**: Calculates the exact amount of color tubes and developer needed for a standard coloring application
- **get_strand_test_recommendation**: Provides safety and efficacy guidance based on the delta between current and target levels


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hair Dye Formulation Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have long, coarse hair at level 4. I want to go to level 7 using a permanent color. How much product do I need?"

**🤖 AI Agent:**
> For long, coarse hair at level 4 moving to level 7, you will need 3 tubes of color (180ml) and 180ml of developer for a 1:1 permanent application.

---

**👤 You:**
> "Calculate a bleach mixture for medium length, fine hair with high porosity for a full head application."

**🤖 AI Agent:**
> For medium length, fine hair with high porosity, you will need 48g of bleach powder and 96ml of developer.

---

**👤 You:**
> "Should I do a strand test if I am moving from level 2 to level 6 with high-lift color?"

**🤖 AI Agent:**
> Yes, a strand test is highly recommended because the level difference is 4 and you are using high-lift chemicals, which increases the risk of over-processing.


## ❓ FAQ

**Q: How does the tool account for hair thickness?**
The tool uses thickness to adjust the volume range. Fine hair uses the lower bound of the length-based multiplier, while coarse hair uses the upper bound to ensure full saturation.

**Q: When should I use the bleach mixture tool?**
Use `calculate_bleach_mixture` when you need to lift hair color using bleach powder rather than depositing color with a dye.

**Q: Is a strand test always required?**
A strand test is recommended by `get_strand_test_recommendation` if the difference between your current and target color level is greater than 3, or if you are using high-lift chemicals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/hair-dye-formulation-calculator](https://vinkius.com/ai-agent-connect/hair-dye-formulation-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hair Dye Formulation Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hair-dye-formulation-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hair Dye Formulation Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hair-dye-formulation-calculator": {
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
