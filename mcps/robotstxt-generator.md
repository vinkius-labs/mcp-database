# Robots.txt Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/robotstxt-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automation](../categories/automation.md)

Generate syntactically valid robots.txt files by configuring user-agent rules, crawl delays, and sitemap URLs.

## Description
The Robots.txt Generator is a configuration-driven engine designed to produce precise instructions for web crawlers. By defining specific rules for different user-agents, you can control how bots like Googlebot or Bingbot interact with your site. Use `generate_robots_txt` to create the final file content, `validate_rule_namespace` to check for syntax errors in your paths, and `get_configuration_summary` to audit your current rule complexity. This tool ensures that all directives follow the standard protocol, including proper handling of 'Allow', 'Disallow', 'Crawl-delay', and 'Sitemap' pointers.


## Available Tools (3)
- **generate_robots_txt**: Generates a robots.txt file based on agent rules
- **get_configuration_summary**: Provides a summary of the current robots.txt configuration
- **validate_rule_syntax**: Validates the syntax of robots.txt rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Robots.txt Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a robots.txt file for all bots that disallows the '/private/' directory and includes a sitemap at https://mysite.com/sitemap.xml."

**🤖 AI Agent:**
> User-agent: *
Disallow: /private/

Sitemap: https://mysite.com/sitemap.xml

---

**👤 You:**
> "Create rules for Googlebot to allow '/images/' but disallow '/temp/', with a crawl delay of 10 seconds."

**🤖 AI Agent:**
> User-agent: Googlebot
Disallow: /temp/
Allow: /images/
Crawl-delay: 10

---

**👤 You:**
> "Check if my rules for 'BadBot' are valid: agentName: 'BadBot', disallowedPaths: ['/api/v1/'], allowedPaths: []"

**🤖 AI Agent:**
> The syntax for the rules provided is valid.


## ❓ FAQ

**Q: How do I generate a new robots.txt file?**
Use the `generate_robots_txt` tool by providing an array of agent rules containing names, allowed paths, and disallowed paths.

**Q: Can I validate my rules before generating the file?**
Yes, you can use the `validate_rule_syntax` tool to check for illegal characters or improper formatting in your rule sets.

**Q: How do I see a summary of my current configuration?**
You can call the `get_configuration_summary` tool to get an overview of how many agents are defined and if a sitemap is included.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/robotstxt-generator](https://vinkius.com/mcp/robotstxt-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Robots.txt Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `robotstxt-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Robots.txt Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "robotstxt-generator": {
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
