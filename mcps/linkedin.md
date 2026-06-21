# LinkedIn MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linkedin)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your LinkedIn presence — audit organizations, posts, and profile via AI.

## Description
Empower your AI agent to orchestrate your entire professional ecosystem on **LinkedIn**, the world's largest professional network. By connecting LinkedIn to your agent, you transform professional networking and publishing into a natural conversation. Your agent can instantly list your administered organizations, audit recent posts, and create new content without you ever touching a dashboard. Whether you are building a personal brand or managing a corporate page, your agent acts as a real-time professional assistant, ensuring your presence is always active and your networking data is organized.

### What you can do

- **Post Distribution** — Create and publish new posts (UGC) directly to your profile or administered organization pages.
- **Organization Oversight** — List all organizations where you have administrative access and retrieve detailed metadata.
- **Content Auditing** — Query recent posts for any author URN to stay on top of your content strategy and engagement.
- **Profile Intelligence** — Retrieve detailed authenticated user info and primary email to ensure organizational alignment.
- **URN Management** — Quickly identify unique identifiers (URNs) for people and organizations to facilitate precise API operations.

### How it works

1. Subscribe to this server
2. Enter your LinkedIn Access Token
3. Start managing your professional workflow through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Thought Leaders** — publish insights and updates straight from your professional workflow.
- **Marketing Managers** — verify if new posts have been correctly published on organization pages.
- **Recruiters & Sales** — perform rapid audits of organization profiles and monitor content distribution.
- **Operations Leads** — automate professional data querying to orchestrate cross-functional outreach teams smoothly.


## Available Tools (6)
- **create_post**: Create a new post (UGC) on LinkedIn
- **get_email**: Get primary email address of the authenticated user
- **get_me**: Get authenticated user info from LinkedIn
- **get_organization**: Get details for a specific organization
- **list_organizations**: List organizations where the user is an administrator
- **list_posts**: List recent posts for an author


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LinkedIn** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get my LinkedIn profile and email."

**🤖 AI Agent:**
> I've retrieved your profile. You are 'Marcus R.' and your primary email is 'marcus@vinkius.com'. Would you like to see your administered organizations?

---

**👤 You:**
> "List all organizations I manage on LinkedIn."

**🤖 AI Agent:**
> I've found 2 organizations where you are an administrator: 'Vinkius Labs' and 'Growth Tech'. Which one would you like the details for?

---

**👤 You:**
> "Create a public post on my profile: 'Excited to launch our new MCP servers!'"

**🤖 AI Agent:**
> Post created successfully! Your update is now live on your profile with visibility set to PUBLIC. I've recorded the post URN for your audit.


## ❓ FAQ

**Q: How do I find my LinkedIn Access Token?**
Create a developer account at [**developer.linkedin.com**](https://developer.linkedin.com/), create an App, and perform the OAuth 2.0 flow to generate a token with the required permissions. Copy and paste it below.

**Q: Can the agent post to my company page?**
Yes. Use the `create_post` tool providing the organization's URN as the author. Your agent will publish the content and confirm the status instantly.

**Q: Is it possible to see my primary email via the agent?**
Yes. The `get_email` tool allows your agent to retrieve the primary email address associated with your LinkedIn account, ensuring your profile data is accurate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linkedin](https://vinkius.com/mcp/linkedin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LinkedIn** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `linkedin` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LinkedIn** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "linkedin": {
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
