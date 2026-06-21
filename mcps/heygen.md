# HeyGen MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/heygen)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Automate AI video generation via HeyGen — manage avatars, videos, and templates directly from any AI agent.

## Description
Connect your **HeyGen** account to any AI agent and take full control of your AI-powered video production and avatar management through natural conversation.

### What you can do

- **Avatar Oversight** — List all available avatars, including public, instant, and custom photo avatars.
- **Video Generation** — Trigger studio-quality video generation tasks by providing scenes and avatar configurations.
- **Template Automation** — Create personalized videos at scale by replacing variables in pre-designed templates.
- **Status Tracking** — Monitor the progress of your video generation tasks and retrieve final URLs when ready.
- **Video Translation** — Automatically translate existing videos into multiple languages with seamless lip-syncing.
- **History & Analytics** — Browse your history of generated videos and interactive streaming sessions.

### How it works

1. Subscribe to this server
2. Enter your HeyGen API Key (found in User Settings > Developer)
3. Start generating AI videos from Claude, Cursor, or any MCP-compatible client

No more manual configuration in the studio for every video. Your AI assistant acts as a dedicated Video Producer or Creative Director.

### Who is this for?

- **Content Creators** — instantly generate talking head videos for social media or training without a camera.
- **Marketing Teams** — automate personalized video outreach at scale using templates.
- **Learning & Development** — quickly update and translate training content for global teams.


## Available Tools
- **generate_from_template**: Pass the variable mapping as a JSON string in "variables_json".

Create a video by replacing variables in a template
- **generate_video**: Pass the scenes and avatar configuration as a JSON string in "body_json" (e.g., {"video_inputs": [...]}).

Manually trigger studio video generation
- **get_api_profile**: Get information about the current API account
- **get_template_details**: Get structure and variable definitions for a specific template
- **get_video_status**: Returns "completed" with a "video_url" when ready.

Check the status and retrieve the URL of a generated video
- **list_avatar_groups**: List categorized groups of avatars
- **list_avatars**: Use this to find the "avatar_id" for video generation.

List all available HeyGen avatars
- **list_streaming_history**: List history of interactive streaming sessions
- **list_templates**: List all video templates
- **list_videos**: List history of generated videos
- **translate_video**: Pass the configuration as a JSON string in "body_json".

Translate an existing video into another language with lip-sync


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HeyGen** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available avatars and find one named 'Joshua'."

**🤖 AI Agent:**
> I've retrieved the list of avatars. I found 'Joshua in Suit' (ID: joshua_v3) and 'Joshua Casual'. Would you like to use one of these for a video generation task?

---

**👤 You:**
> "Show me the status of video ID 'vid_99283'."

**🤖 AI Agent:**
> Checking video status... Your video 'vid_99283' is currently COMPLETED. You can watch it or download it here: [Watch Video](https://heygen.com/video/...) Should I retrieve your full video history?

---

**👤 You:**
> "Generate a video from template 'welcome_v1' with variable {'name': 'John Doe'}."

**🤖 AI Agent:**
> Template generation triggered! I've started the production of your video using the 'welcome_v1' template. This usually takes 2-5 minutes. I'll monitor the status for you. Should I notify you once the URL is ready?


## ❓ FAQ

**Q: How do I find my HeyGen API Key?**
Log in to your HeyGen account, navigate to **User Settings**, and select the **Developer** tab. You will be able to generate and copy your unique API key from there.

**Q: How can I generate a video using a template?**
First, use `list_templates` to find the template you want. Then, use the `generate_from_template` tool by providing the template ID and a JSON string mapping the variables (like text or image URLs) you want to replace.

**Q: Can I translate existing videos into other languages?**
Yes! Use the `translate_video` tool. You must provide the source video URL and the target language code. HeyGen will generate a new version of the video with the translated audio and lip-syncing.

**Q: Is the integration secure for creative data?**
Absolutely. The integration uses official HeyGen API keys over HTTPS. Your credentials are encrypted and stored securely within the Vinkius Cloud infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/heygen](https://vinkius.com/mcp/heygen)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HeyGen** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `heygen` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HeyGen** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "heygen": {
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
