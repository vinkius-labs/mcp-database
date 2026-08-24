# Espresso Extraction Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/espresso-extraction-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate espresso extraction yield, brew ratio, and dose adjustments.

## Description
A precision tool for baristas to optimize espresso profiles. Use `analyze_extraction` to evaluate current yield and strength, or `calculate_dose_adjustment` to find the exact dose needed to hit a target extraction yield. This MCP connects your AI assistant to professional brewing mathematics.


## Available Tools (3)
- **calculate_dose_adjustment**: 
- **validate_extraction_parameters**: 
- **analyze_extraction**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Espresso Extraction Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I used 18g of coffee to get 36g of espresso with a TDS of 9%. What is my extraction yield?"

**🤖 AI Agent:**
> Your extraction yield is 18.0%, which is considered an ideal extraction.

---

**👤 You:**
> "My current dose is 20g, but I want to hit a 21% yield with a 40g beverage and 10% TDS. What should my new dose be?"

**🤖 AI Agent:**
> To hit a 21% yield, your new dose should be 21.0g, which is an increase of 1.0g.

---

**👤 You:**
> "Is a 5g dose for a 40g espresso shot with 10% TDS valid?"

**🤖 AI Agent:**
> No, that is not a valid extraction as the yield would exceed 100%.


## ❓ FAQ

**Q: How do I know if my espresso is underextracted?**
You can use the `analyze_extraction` tool. If the extraction yield is below 18%, the shot is classified as underextracted, which often tastes sour.

**Q: How can I adjust my dose to reach a target yield?**
Use the `calculate_dose_adjustment` tool. Provide your current dose, the target yield, the beverage weight, and the TDS to find the required dose change.

**Q: What is a realistic TDS for espresso?**
Typically, espresso TDS falls between 6% and 12%. You can use `validate_extraction_parameters` to check if your measurements are within reasonable bounds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/espresso-extraction-calculator](https://vinkius.com/ai-agent-connect/espresso-extraction-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Espresso Extraction Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `espresso-extraction-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Espresso Extraction Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "espresso-extraction-calculator": {
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
