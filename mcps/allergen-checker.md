# Allergen Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/allergen-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Scan ingredients and recipes for the 14 mandatory allergens.

## Description
The Allergen Checker MCP server provides a critical safety layer for food preparation and analysis. By using tools like `ingredient_check`, `recipe_safety_check`, and `allergen_reference`, users can instantly identify potential health risks in ingredients or entire recipes based on the 14 mandatory allergens regulated by EU and Brazilian laws. The system detects common derivatives (e.g., identifying 'whey' as a milk allergen) to ensure comprehensive safety reporting.


## Available Tools (3)
- **allergen_reference**: Provides a list of all allergens and their keywords
- **ingredient_check**: Checks a single ingredient for allergens
- **recipe_safety_check**: Analyzes a whole recipe for allergens


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Allergen Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is there any milk in this ingredient: 'whey protein isolate'?"

**🤖 AI Agent:**
> Yes, 'whey protein isolate' contains Milk.

---

**👤 You:**
> "Check this recipe for allergens: ['flour', 'sugar', 'eggs', 'milk']."

**🤖 AI Agent:**
> The recipe is unsafe. Detected allergens: Eggs, Milk.

---

**👤 You:**
> "What are the keywords used to identify peanuts?"

**🤖 AI Agent:**
> Keywords for Peanuts include: 'peanut', 'groundnut'.


## ❓ FAQ

**Q: How does the allergen detection work?**
The system scans ingredient text for keywords associated with 14 mandatory allergens and their common derivatives, such as identifying 'casein' as a milk allergen.

**Q: Can I check an entire recipe at once?**
Yes, use the `recipe_safety_check` tool by providing a JSON array of all ingredients in your recipe to get a summarized safety report.

**Q: What allergens are covered?**
The tool covers the 14 mandatory allergens regulated by EU and Brazilian food safety laws, including Milk, Gluten, Soybeans, Eggs, Peanuts, Tree Nuts, Crustaceans, Fish, Celery, Mustard, Sesame Seeds, Sulphites, Lupin, and Molluscs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/allergen-checker](https://vinkius.com/mcp/allergen-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Allergen Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `allergen-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Allergen Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "allergen-checker": {
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
