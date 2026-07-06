# Gelatin Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gelatin-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Calculates precise gelatin amounts for any liquid volume and classifies the resulting texture (mousse, panna cotta, or firm jelly). Standardizes measures between sheets and powder.

## Description
**Need to set a dessert but aren't sure how much gelatin to use?** The final texture of your mousse, panna cotta, or jelly depends on the precise ratio of gelatin to liquid volume--a relationship often misunderstood. Using too little results in failure; using too much results in an overly firm structure. Our tool solves this by establishing a scientifically accurate calculation mechanism.


## Available Tools (3)
- **calculate_required_gelatine**: Takes liquid volume in milliliters and a firmness profile (mousse, panna_cotta, or firm_jelly) to determine the precise gelatin amount required.

Calculate how much gelatin is needed for a given liquid volume and desired firmness
- **gelatine_conversion_factor**: Input form is "sheet" or "powder", input value is the measured amount.

Convert between gelatin sheet and powder forms
- **map_gelatine_type**: Takes the target amount in grams equivalent and preferred input form.

Get practical preparation instructions for a calculated gelatin amount


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gelatin Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am making 2 liters of panna cotta. I prefer using powder."

**🤖 AI Agent:**
> Step 1: Use `calculate_required_gelatine` with 2000ml and 'panna_cotta' to get the required amount (e.g., 60g equivalent). Step 2: Use `map_gelatine_type` with 60 and 'powder' for mixing instructions. The final set will be creamy, holding its shape well.

---

**👤 You:**
> "I have 15 sheets of gelatin and need to calculate how many grams that is for my recipe."

**🤖 AI Agent:**
> The `gelatine_conversion_factor` tool will standardize this. It calculates the equivalent powder mass, giving you a precise measurement in grams that can be used in volume calculations.

---

**👤 You:**
> "I need to make a very firm jelly from 100ml of liquid. I use sheets."

**🤖 AI Agent:**
> First, `calculate_required_gelatine` for 100ml and 'firm_jelly' (e.g., 5g equivalent). Then, `map_gelatine_type` with 5 and 'sheet'. This ensures structural integrity suitable for slicing.


## ❓ FAQ

**Q: I only have gelatin sheets, but the recipe calls for powder. How do I calculate the equivalent amount?**
Use the `gelatine_conversion_factor` tool first. This function standardizes your measurement, converting sheets to their powdered mass equivalent (grams). Once you have that standardized amount, use it in subsequent steps.

**Q: I want a light mousse for 500ml of liquid. How much gelatin do I need?**
This is the core function of `calculate_required_gelatine`. Provide the total volume (500ml) and select 'mousse' as your desired firmness profile. The tool will return a precise, recommended amount based on scientific ratios.

**Q: After calculating the needed amount, how do I actually mix it?**
The `map_gelatine_type` tool provides practical preparation instructions. You must provide both the calculated mass equivalent and your preferred input form ('sheet' or 'powder') to get accurate, step-by-step mixing guides.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gelatin-converter](https://vinkius.com/mcp/gelatin-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gelatin Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gelatin-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gelatin Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gelatin-converter": {
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
