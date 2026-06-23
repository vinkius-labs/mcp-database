# Colossyan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/colossyan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate AI video creation via Colossyan — generate videos from templates, manage avatars, and track rendering jobs directly from any AI agent.

## Description
Connect your **Colossyan** account to any AI agent to streamline your synthetic media production. Create high-quality videos with AI avatars using natural language commands.

### What you can do

- **Avatar & Voice Management** — List all available Studio, Scenario, and Instant avatars, or create new ones from source URLs. Explore hundreds of voices across different languages and styles.
- **Video Generation** — Trigger video renders using saved templates with dynamic variables or submit full JSON descriptors for custom creative control.
- **Job Tracking** — Monitor the real-time status of your video generation jobs (queue, generating, finished) and retrieve final public URLs and metadata.
- **Content Lifecycle** — Manage your library by retrieving details of finished videos or deleting jobs and assets when they are no longer needed.
- **Drafting** — Use experimental features to generate video drafts from structured textual summaries.

### How it works

1. Subscribe to this server
2. Enter your Colossyan API Key
3. Start generating AI videos from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Teams** — scale personalized video campaigns by injecting dynamic variables into templates via AI.
- **L&D Professionals** — quickly update training materials and list available actors to find the right fit for educational content.
- **Content Creators** — automate the technical side of video rendering and asset management directly from a chat interface.


## Available Tools (10)
- **create_actor**: Create an instant avatar from an image or video link
- **delete_job**: Delete a video generation job
- **delete_video**: Delete a generated video
- **generate_draft**: Generate a draft from structured textual data (Knowledge to Draft)
- **generate_from_template**: Generate a video using a saved template
- **generate_video**: Generate a video manually using a full JSON descriptor
- **get_job_status**: Retrieve video generation job status
- **get_video**: Retrieve details of a finished video
- **list_actors**: List available avatars/actors for the workspace
- **list_voices**: List available voices for the workspace


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Colossyan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available AI actors and voices in my Colossyan account."

**🤖 AI Agent:**
> I've retrieved your available assets. You have access to 15 Studio actors and 42 voices across 10 languages. Would you like to see the details for a specific language or actor type?

---

**👤 You:**
> "Generate a video from template 'tpl_9988' with the variable name set to 'Sarah'."

**🤖 AI Agent:**
> Starting video generation using template 'tpl_9988'. I've mapped the dynamic variable 'name' to 'Sarah'. The job ID is `vid_conf_123`. I'll monitor the status for you.

---

**👤 You:**
> "Check the status and get the link for video ID 'vid_conf_123'."

**🤖 AI Agent:**
> The video generation for `vid_conf_123` is finished! You can view it here: [Public URL]. The video is 45 seconds long and ready for download.


## ❓ FAQ

**Q: How can I check if my video has finished rendering?**
You can use the `get_job_status` tool by providing the `videoId`. The agent will return the current status, such as 'finished', 'generating', or 'failed'.

**Q: Can I generate videos using my existing Colossyan templates?**
Yes! Use the `generate_from_template` tool. You'll need the `templateJobId` and a JSON object for `dynamicVariables` to fill in the placeholders in your template.

**Q: How do I see which AI avatars are available in my account?**
Simply ask the agent to run the `list_actors` tool. It will retrieve all available avatars, including Studio, Scenario, and Instant types configured for your workspace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/colossyan](https://vinkius.com/mcp/colossyan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Colossyan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `colossyan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Colossyan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "colossyan": {
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
