# Canny MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/canny)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Manage product feedback via Canny — track feature requests, bugs, and user votes directly from any AI agent.

## Description
Connect your **Canny** account to any AI agent and orchestrate your product feedback, roadmap prioritization, and community engagement through natural conversation.

### What you can do

- **Post Oversight** — List and retrieve detailed metadata for all feedback items (ideas, feature requests, bugs) across your boards.
- **Roadmap Coordination** — Monitor the status of posts (Planned, In-Progress, Complete) to stay aligned with your product strategy.
- **Community Engagement** — Add votes and comments to posts directly from your workspace to interact with user feedback.
- **Board Management** — List all feedback boards and retrieve their specific configuration and categories.
- **User Tracking** — Access your directory of users who have interacted with your boards to understand your community.
- **Feedback Creation** — Create new posts directly from your workspace with titles, details, and associated authors.

### How it works

1. Subscribe to this server
2. Enter your Canny Secret API Key
3. Start managing your product roadmap from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — quickly triage new feedback or check post statuses without manual dashboard monitoring.
- **Customer Success** — add user votes or retrieve feedback details straight from their communication tools.
- **Developers** — monitor bug reports and feature requests using natural language.


## Available Tools (11)
- **add_comment**: Add a comment to a feedback post
- **create_feedback_post**: Create a new feedback post (idea, bug, etc)
- **vote_on_post**: Add a vote to a feedback post
- **get_account_info**: Retrieve core account information
- **get_board_details**: Get details of a specific board
- **get_post_details**: Get details of a specific feedback post
- **list_feedback_boards**: List all feedback boards
- **list_comments**: List comments for a specific feedback post
- **list_feedback_posts**: List feedback items (posts) from a specific board
- **list_users**: List users who have interacted with your boards
- **list_votes**: List votes for a specific post


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Canny** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active feedback boards in Canny."

**🤖 AI Agent:**
> I've retrieved your boards. You have 3 active boards: 'Feature Requests' (ID: board_1), 'Bug Reports' (ID: board_2), and 'Languages' (ID: board_3).

---

**👤 You:**
> "Show the top 5 most voted posts on the 'Feature Requests' board."

**🤖 AI Agent:**
> Retrieving top posts... The most voted items include 'Dark Mode Support' (Score: 450) and 'Offline Access' (Score: 320). Would you like to see the comments for any of these?

---

**👤 You:**
> "Add a comment 'Great idea!' to post ID 99283 as author user_123."

**🤖 AI Agent:**
> Comment 'Great idea!' has been successfully added to post 99283 in Canny.


## ❓ FAQ

**Q: Can I add a vote to a post using the agent?**
Yes! Use the `vote_on_post` tool with the Post ID and Voter ID. Your agent will add the vote in Canny, helping prioritize the feedback item.

**Q: How do I list all the planned features from a specific board?**
Simply ask the agent to `list_feedback_posts` and provide the Board ID and set the status to `planned`. It will retrieve all matching posts from your Canny account.

**Q: Does the integration allow creating a new feedback post?**
Yes. Use the `create_feedback_post` action and provide the Board ID, Author ID, title, and details. The new item will be added to your Canny board instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/canny](https://vinkius.com/mcp/canny)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Canny** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `canny` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Canny** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "canny": {
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
