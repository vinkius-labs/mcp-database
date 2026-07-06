# Synthesia MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/synthesia)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Connect your AI to Synthesia. Generate corporate AI avatar videos from text prompt, explore templates, and automatically dub existing media directly from the terminal.

## Description
Bring the full power of synthetic enterprise video generation directly into your conversational environment with the **Synthesia** MCP connector. By granting your LLM authorized operational access to the Synthesia API matrix, you transform your assistant into a virtual studio director. Programmatically retrieve active templates, inspect available voice models, spawn new avatar streams from zero, or dub existing media seamlessly without navigating away from your terminal interface.

### What you can do

- **Virtual Directing** — Instantiate real-time video renderings using `create_avatar_video`, mapping structural inputs to specific avatar matrices found via `list_avatars`.
- **Template Automation** — Process repetitive layouts logically calling `create_video_from_template`, assigning JSON payloads seamlessly over defined blueprints.
- **Studio Lifecycle Management** — Query active rendering progress cleanly with `get_video_details` and prune discarded tracks strictly invoking `delete_video`.
- **Localization & Dubbing** — Effortlessly pull native voice ranges (`list_voices`) and trigger AI localized dubbing routines targeting existing records utilizing `dub_video`.

### How it works

1. Append the generic Synthesia MCP module firmly inside your Vinkius connective logic rules.
2. Locate your specific account authorization `SYNTHESIA_KEY` (tied to Synthesia Creator plans and beyond) and pass it to your host configuration.
3. Prompt video creations natively: "List all available avatars, pick a professional-looking one, and generate a video track saying 'Welcome to the Team!' in 'pt-BR'."

### Who is this for?

- **Corporate Training Leads** — Programmatically dispatch multi-lingual instructional videos evaluating template arrays generating bulk outputs seamlessly.
- **Internal Comms Engineers** — Eliminate manual studio workflows assigning custom scripts strictly inside automated pipelines using the AI interface directly.
- **Localization Teams** — Rapidly inspect voice definitions natively scaling video catalogs commanding dynamic `dub_video` requests effortlessly.


## Available Tools (10)
- **create_video_from_template**: Returns a video ID.

Creates a video using a pre-defined Synthesia template
- **get_video_details**: Retrieves status and details for a specific video
- **list_videos**: Lists all videos in the account
- **delete_video**: This action is irreversible.

Permanently deletes a Synthesia video
- **list_avatars**: Lists all available AI avatars
- **list_templates**: Lists available video templates
- **get_template_details**: Retrieves details for a specific template
- **list_voices**: Lists available AI voices
- **dub_video**: Dubs an existing video into another language
- **create_avatar_video**: Returns a video ID.

Creates an AI avatar video from a script


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Synthesia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a list of internal AI video templates, select one related to 'customer support', and execute a creation pass using proper test inputs."

**🤖 AI Agent:**
> Accessing Synthesia directories ('list_templates')...
Found template 'Support Starter' (ID: tmpl-1234).
Fetching target blueprint variables natively ('get_template_details').
Dispatching 'create_video_from_template' with payload values successfully...
Video task submitted. The ID is 'vid-5678'. Let me know when you want to execute 'get_video_details'.

---

**👤 You:**
> "List the available AI avatars, focusing on professional corporate styles."

**🤖 AI Agent:**
> Querying Synthesia avatar registry ('list_avatars')...
Here are some of the active top corporate avatars available for rendering:
1. 'Anna_Business' (ID: 101) - Blazer, formal.
2. 'Marcus_Exec' (ID: 105) - Suit, authoritative.
3. 'Elena_Office' (ID: 112) - Smart casual, friendly.

---

**👤 You:**
> "Check the status of my recent video task 'vid-9920'."

**🤖 AI Agent:**
> Evaluating task bounds ('get_video_details')...
The render for 'vid-9920' is COMPLETE. 
Total duration: 45 seconds.
You can download and stream the final file here: `https://synthesia.io/stream/vid-9920_xyz`.


## ❓ FAQ

**Q: How long does video rendering take?**
The `create_avatar_video` command submits the job instantly. Rendering typically takes 2–10 minutes depending on length. Use `get_video_details` to check progress and retrieve the final URL.

**Q: Can I use my custom avatars?**
Yes. The `list_avatars` tool returns both stock and custom avatars tied to your account. You can use any avatar ID when creating videos.

**Q: Which Synthesia plan is required?**
API access requires a Creator or Enterprise plan. Free and Starter plans do not include API keys. Check the Integrations tab in your Synthesia dashboard to verify eligibility.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/synthesia](https://vinkius.com/mcp/synthesia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Synthesia** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `synthesia` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Synthesia** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "synthesia": {
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
