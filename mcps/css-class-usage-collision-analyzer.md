# CSS Class Usage & Collision Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/css-class-usage-collision-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [development](../categories/development.md)

Identify orphaned, missing, or colliding CSS classes in your project.

## Description
This MCP server provides static analysis for frontend projects to maintain clean and predictable stylesheets. It maps CSS/SCMS class definitions to their usage in HTML/JSX, allowing you to find `find_orphaned_classes` (defined but unused), `find_broken_references` (used but undefined), and `find_css_collisions` (duplicate definitions across files).


## Available Tools (3)
- **find_broken_references**: html/.jsx/.tsx files and checks if each class has a corresponding definition in .css/.scss files.

Identifies class names used in HTML/JSX that lack CSS definitions
- **find_css_collisions**: css/.scss files in the project root to identify if the same class name is defined in multiple places.

Detects duplicate class definitions across different CSS files
- **find_orphaned_classes**: css/.scss files and compares them against usage in .html/.jsx/.tsx files.

Identifies CSS classes that are declared but never used


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CSS Class Usage & Collision Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all unused CSS classes in /path/to/my-project"

**🤖 AI Agent:**
> The analysis found 3 orphaned classes: .btn-unused, .header-for-old, and .footer-deprecated.

---

**👤 You:**
> "Are there any broken class references in my React project?"

**🤖 AI Agent:**
> Yes, the following classes are used but not defined: .missing-style and .undefined-class.

---

**👤 You:**
> "Check for CSS class collisions in /workspace/app"

**🤖 AI Agent:**
> A collision was detected for class '.card-title' which is defined in both globals.css and component.module.css.


## ❓ FAQ

**Q: What does `find_orphaned_classes` do?**
It identifies CSS classes that are declared in your stylesheets but have no corresponding usage in your HTML or JSX files.

**Q: How can I detect broken class references?**
Use the `find_broken_references` tool to find class names used in your components that do not exist in any scanned stylesheet.

**Q: Can this tool detect duplicate CSS definitions?**
Yes, the `find_css_collisions` tool detects when the same class name is defined in multiple different CSS or SCSS files.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/css-class-usage-collision-analyzer](https://vinkius.com/mcp/css-class-usage-collision-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CSS Class Usage & Collision Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `css-class-usage-collision-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CSS Class Usage & Collision Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "css-class-usage-collision-analyzer": {
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
