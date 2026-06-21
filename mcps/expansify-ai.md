# Expansify AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/expansify-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Scale your content marketing with AI that generates, repurposes, and distributes content across channels automatically.

## Description
Connect your **Expansify AI** account to any AI agent and take full control of your content marketing and SEO workflows through natural conversation.

### What you can do

- **Campaign Orchestration** — List and manage all AI content campaigns and retrieve detailed metadata about strategy and performance programmatically
- **Automated Content Generation** — Programmatically generate blog posts, social media updates, and ad copy by providing prompts and content types directly through your agent
- **SEO Intelligence** — List and monitor tracked SEO keywords to maintain a high-fidelity oversight of your search engine visibility
- **Keyword Analysis** — Trigger deep SEO analysis for specific keywords to optimize your content strategy and identify ranking opportunities
- **Content Library Navigation** — Access the complete history of generated AI content to reuse or refine previous marketing materials

### How it works

1. Subscribe to this server
2. Retrieve your **API Token** from your Expansify AI dashboard (Settings > API Keys)
3. Start generating and optimizing marketing content from Claude, Cursor, or any MCP client

No more manual copy-pasting or switching between tools to check SEO rankings. Your AI acts as your dedicated content strategist and SEO coordinator.

### Who is this for?

- **Content Marketers** — instantly launch new content campaigns and generate copy using natural language queries
- **SEO Specialists** — monitor keyword rankings and perform technical analysis without leaving your workspace
- **Growth Teams** — automate the creation of ad variants and social posts through simple AI commands


## Available Tools
- **analyze_keyword_seo**: Analyze a keyword for SEO
- **create_campaign**: Create a new content campaign
- **generate_ai_content**: ).

Generate new AI content
- **list_campaigns**: List all AI content campaigns
- **list_generated_content**: List generated AI content
- **list_tracked_keywords**: List tracked SEO keywords


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Expansify AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a blog post about 'The future of RAG in 2026' using Expansify AI."

**🤖 AI Agent:**
> Generating content... I've written a blog post draft focusing on advanced RAG techniques and AI integration. You can find the full text in your content history with ID: gen_123.

---

**👤 You:**
> "List all my active content campaigns."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 3 active drives: 'Q1 Tech Strategy', 'Social Engagement', and 'Ad Copy Variations'. Which one should we manage?

---

**👤 You:**
> "Analyze the SEO difficulty for the keyword 'mcp server implementation'."

**🤖 AI Agent:**
> SEO analysis complete! The keyword 'mcp server implementation' has a moderate difficulty score (45/100). It's a high-intent term with growing search volume. Shall I suggest some related long-tail keywords?


## ❓ FAQ

**Q: How do I find my API Token?**
Log in to your Expansify AI account and navigate to **Settings** > **API Keys** to generate and copy your unique access token.

**Q: Can the agent generate different types of content?**
Yes! Use the `generate_ai_content` tool and specify the `type` parameter (e.g., blog_post, tweet, ad) along with your topic prompt.

**Q: How do I check the performance of an SEO keyword?**
Use the `analyze_keyword_seo` tool to trigger a technical analysis of any specific keyword to understand its difficulty and ranking potential.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/expansify-ai](https://vinkius.com/mcp/expansify-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Expansify AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `expansify-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Expansify AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "expansify-ai": {
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
