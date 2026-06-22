# Wine Pairing Matcher MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wine-pairing-matcher)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Get expert wine recommendations based on dish characteristics like protein, sauce weight, and intensity.

## Description
The Wine Pairing Matcher uses classical principles of structural symmetry to suggest the perfect wine for any dish. By analyzing the protein type, sauce weight, and overall flavor intensity, it identifies wines that complement or contrast with your meal effectively. Use `match_wine_to_dish` to find a specific style, `check_pairing_risk` to avoid palate clashes, or `get_protein_guidines` to learn the foundational rules for different proteins.


## Available Tools (3)
- **check_pairing_risk**: Evaluates if a specific wine style will clash negatively with a dish component
- **match_wine_to_dish**: Provides a specific wine style recommendation for a given dish configuration
- **get_protein_guidelines**: Retrieves the foundational wine pairing principles for a specific protein type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Pairing Matcher** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What wine should I pair with a beef steak with a heavy red wine reduction and robust spices?"

**🤖 AI Agent:**
> A Full-bodied Red is recommended. The high tannins in the wine will complement the protein and fat, while the intensity matches the robust spice profile.

---

**👤 You:**
> "Is a light white wine risky for a dish with salmon in a heavy cream sauce?"

**🤖 AI Agent:**
> There is a High risk of palate clashing. The high fat content of the heavy sauce may overwhelm a light, acidic wine.

---

**👤 You:**
> "What are the general pairing guidelines for seafood?"

**🤖 AI Agent:**
> For seafood, you should look for wines with High acidity, Low tannins, and a Light body to avoid overpowering the delicate protein.


## ❓ FAQ

**Q: How does the pairing logic work?**
The engine uses 'structural symmetry'. It matches the weight and intensity of a wine to the dish. For example, heavy proteins like beef pair with high-tannin wines, while delicate seafood requires high acidity.

**Q: Can I check if a specific wine will clash with my meal?**
Yes, use the `check_pairing_risk` tool. It evaluates potential clashes between your protein type, sauce weight, and a specific wine style.

**Q: What inputs are required for a recommendation?**
To use `match_wine_to_dish`, you need to provide the protein type (e.g., beef, fish), the sauce weight (light, medium, or heavy), and the dish intensity (delicate, moderate, or robust).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wine-pairing-matcher](https://vinkius.com/mcp/wine-pairing-matcher)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Pairing Matcher** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-pairing-matcher` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Pairing Matcher** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-pairing-matcher": {
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
