# Copysmith MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/copysmith)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate marketing copy, product descriptions, and ad variations at scale with AI trained on high-performing content.

## Description
Connect your **Copysmith** account to any AI agent and take full control of your marketing content production and AI-driven copywriting workflows through natural conversation.

### What you can do

- **Content Orchestration** — Instantly generate product descriptions, Facebook ads, and blog intros using dozens of pre-built, high-fidelity AI templates
- **Digital Asset Management** — Create and manage folders and files programmatically to maintain a perfectly coordinated content repository
- **Template Intelligence** — Access your complete directory of copywriting templates and retrieve detailed input requirements directly through your agent
- **Usage Monitoring** — Programmatically track your credit balance and account status to coordinate your content production budget
- **Automated Workflow** — Programmatically create generations, retrieve results, and manage your file lifecycle to maintain a structured marketing ecosystem

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Copysmith dashboard (Settings > API)
3. Start scaling your content production from Claude, Cursor, or any MCP client

No more manual copy-pasting between chat windows. Your AI acts as your dedicated marketing copywriter and content coordinator.

### Who is this for?

- **E-commerce Owners** — instantly generate bulk product descriptions and ad copy using natural language commands
- **Content Marketers** — automate the creation of blog outlines and intros without leaving your workspace
- **Agencies** — orchestrate client content across multiple folders and monitor credit utilization through simple AI queries


## Available Tools (12)
- **create_folder**: Create a new folder
- **create_generation**: Generate AI content
- **delete_file**: Delete a file
- **delete_folder**: Delete a folder
- **get_credits**: Check remaining credits
- **get_file**: Get file details
- **get_generation**: Get generation status
- **get_template**: Get template details
- **get_user_info**: Get user details
- **list_files**: Can be filtered by folder.

List files
- **list_folders**: List all folders
- **list_templates**: g., Product Description, Blog Intro).

List all content templates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Copysmith** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a product description for 'AI Project Manager' using the 'Product Description' template."

**🤖 AI Agent:**
> Generation triggered! I've started creating your product description for 'AI Project Manager'. The job ID is 'gen_123'. I'll retrieve the finalized copy for you as soon as it's ready.

---

**👤 You:**
> "Show me all my content folders and files in Copysmith."

**🤖 AI Agent:**
> I've retrieved your content hierarchy. You have 2 folders: 'Q1 Campaigns' and 'Drafts', with a total of 15 saved files. Which one would you like to inspect?

---

**👤 You:**
> "Check my remaining credits balance."

**🤖 AI Agent:**
> Scanning account... You have 1,240 credits remaining. Based on your current usage, you can generate approximately 50 more high-quality articles. Need any help with a new campaign?


## ❓ FAQ

**Q: How do I find my Copysmith API Key?**
Log in to your account, navigate to **Settings** > **API**, and copy your secret access token from the dashboard.

**Q: How many credits are used per generation?**
Credit consumption depends on the complexity and length of the content generated. You can check your balance using the `get_credits` tool.

**Q: Can I list available templates via AI?**
Yes! The `list_templates` tool retrieves all active copywriting models available for your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/copysmith](https://vinkius.com/mcp/copysmith)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Copysmith** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `copysmith` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Copysmith** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "copysmith": {
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
