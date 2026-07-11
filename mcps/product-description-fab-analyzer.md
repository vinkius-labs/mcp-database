# Product Description FAB Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/product-description-fab-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Audit your product copy for Feature-Advantage-Benefit (FAB) structural integrity and persuasive impact.

## Description
The Product Description FAB Analyzer scans your text to identify Features, Advantages, and Benefits. By using `analyze_sentence_structure`, it classifies every sentence in your copy. You can then use `calculate_copy_metrics` to find your feature-to-benefit ratio and benefit density score. Finally, `generate_copy_audit` provides a high-level verdict on whether your copy is optimal or critically unbalanced. This tool helps copywriters ensure their technical specifications are always connected to user value.

### Available Tools

`analyze_product_description`


## Available Tools (1)
- **analyze_product_description**: Analyze a product description using the FAB (Features, Advantages, Benefits) framework


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Product Description FAB Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this copy: "Our shoes are made of leather. They are durable. You will love them.""

**🤖 AI Agent:**
> The analysis shows a feature (leather), an advantage (durable), and a benefit (you will love them). Your feature-to-benefit ratio is 1:1.

---

**👤 You:**
> "Check the metrics for this text: "This drill has a brushless motor. It lasts longer. It's great.""

**🤖 AI Agent:**
> The `calculate_copy_metrics` tool reports a high benefit density score and an optimal specification-vs-narrative ratio.

---

**👤 You:**
> "Generate an audit for: "The battery lasts 20 hours. It is lightweight.""

**🤖 AI Agent:**
> The `generate_copy_audit` tool provides a verdict of 'functional' with a primary issue of unmatched features due to the lack of a benefit statement.


## ❓ FAQ

**Q: What is the FAB framework?**
It stands for Features, Advantages, and Benefits, a method to structure persuasive copy. Tools available: `analyze_product_description`.

**Q: How does it identify unmatched features?**
The `analyze_sentence_structure` tool flags features that lack a corresponding benefit or advantage in the text.

**Q: Can I use this for SEO optimization?**
Yes, by improving your benefit density and structural balance, you create more engaging content for users.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/product-description-fab-analyzer](https://vinkius.com/mcp/product-description-fab-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Product Description FAB Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `product-description-fab-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Product Description FAB Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "product-description-fab-analyzer": {
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
