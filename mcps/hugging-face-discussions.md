# Hugging Face Discussions MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hugging-face-discussions)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Transform the world's largest ML hub into your growth engine. Deploy autonomous agents to intercept trending discussions and engage the AI elite in real-time.

## Description
Empower your AI agent to orchestrate your entire community interaction on Hugging Face with **Hugging Face Discussions**, the hub for the world's machine learning developers. By connecting this Vinkius toolset to your agent, you transform complex reconnaissance into a natural, strategic conversation. Your agent can instantly scan trending repositories, audit community discussions, and find exact threads where developers are discussing specific topics (like 'tool-calling' or 'deployment errors'). Whether you are tracking the latest LLMs or providing support for your own models, your agent acts as a real-time community manager, ensuring you intercept the most valuable conversations.

### What you can do

- **Targeted Reconnaissance** — Scan top trending repositories and search their active discussions for specific keywords to find high-value interception points.
- **Intelligence Reports** — Get a consolidated view of repository statistics combined with top open discussions for rapid situational awareness.
- **Repository Search** — Search for specific models, datasets, or spaces based on current hype.
- **Community Engagement** — Read discussion threads and post replies automatically, providing technical solutions or support right where developers are looking for them.
- **Discussion Creation** — Open new discussions or issues programmatically to report bugs or request features.

### How it works

1. Subscribe to this Vinkius integration
2. Enter your Hugging Face Access Token (with read/write permissions for discussions)
3. Start monitoring and engaging via your preferred Vinkius-powered agent or compatible client

### Who is this for?

- **AI Infrastructure Providers** — scan for users asking how to test or deploy models, and organically suggest your infrastructure.
- **Model Creators** — monitor issues and discussions across all your repositories without manual checks.
- **Developer Advocates** — find discussions related to your specific stack and engage with the community naturally.
- **Growth Leads** — perform rapid audits of trending models and their pain points.


## Available Tools (8)
- **comment_discussion**: Use Markdown formatting.

Add a comment to an existing Hugging Face discussion
- **create_discussion**: Ensure the title is clear and the description provides all necessary context.

Create a new discussion or issue in a Hugging Face repository
- **get_discussion_details**: You MUST read the discussion details before engaging or commenting to fully understand the context.

Get the full details and comments of a specific Hugging Face discussion
- **get_repo_intelligence**: Use this for rapid market awareness before deciding to engage.

Get a comprehensive intelligence report for a Hugging Face repository
- **get_trending_repositories**: Essential for understanding community interests and providing timely, relevant engagement.

Get the top trending repositories on Hugging Face
- **scan_target_discussions**: Use this to find relevant discussions based on targeted keywords across the most active projects.

Scan trending Hugging Face repositories for discussions matching a specific keyword
- **search_repositories**: Useful for identifying high-value community engagement opportunities based on keywords.

Search for Hugging Face repositories (models, datasets, spaces)
- **get_repo_discussions**: Use this to monitor community activity and identify pain points.

Get discussions/issues for a specific Hugging Face repository


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hugging Face Discussions** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find discussions about 'tool-calling' in trending models."

**🤖 AI Agent:**
> I scanned 10 trending models and found 2 active discussions about 'tool-calling'. In 'meta-llama/Meta-Llama-3-8B' (Issue #142), a user is asking how to implement tool calling. Should I prepare a reply suggesting our Vinkius infrastructure?

---

**👤 You:**
> "Get an intelligence report on the Qwen/Qwen2-72B model."

**🤖 AI Agent:**
> Here is the intelligence report for Qwen/Qwen2-72B: It has over 15,000 likes and 2M downloads this month. There are currently 8 active open discussions. The top discussion is about context window limitations.

---

**👤 You:**
> "Reply to discussion #42 in mistralai/Mistral-7B-v0.1."

**🤖 AI Agent:**
> I've successfully posted your comment to discussion #42. The community will now see your technical breakdown of the infrastructure solution.


## ❓ FAQ

**Q: How do I find my Hugging Face Access Token?**
Go to your Hugging Face account settings, under **Access Tokens**, and create a new fine-grained token. Ensure it has permissions to read and interact with discussions on the specific repositories you want to target.

**Q: Can the agent post replies automatically?**
Yes. Using the `comment_discussion` tool, your agent can write and post Markdown replies directly into community threads.

**Q: How does the target scanning work?**
The `scan_target_discussions` tool fetches the top trending repositories (models, datasets, etc.) and then iterates through their active discussions, filtering for the exact keyword you specify. It's highly efficient for finding interception points.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hugging-face-discussions](https://vinkius.com/mcp/hugging-face-discussions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hugging Face Discussions** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hugging-face-discussions` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hugging Face Discussions** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hugging-face-discussions": {
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
