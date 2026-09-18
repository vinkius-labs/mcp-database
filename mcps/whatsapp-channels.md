# WhatsApp Channels MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/whatsapp-channels)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Post text and media to WhatsApp Channels from any AI agent — create channels, publish posts, search public channels and read their feed.

## Description
Post to WhatsApp Channels from any AI agent through **WAHA**, a free open-source WhatsApp HTTP API you run in Docker on your own server — your WhatsApp session never leaves it.

### What you can do

- **Publish posts** — Send text, image, video or voice posts to any channel where you are owner or admin, with captions and public-file URLs
- **Create channels** — Spin up a new branded channel (name, description, avatar) and get its invite link
- **Discover & monitor** — Search public channels by keyword (explore-style), preview any channel's latest posts with view counts and reactions, and pull full message history from channels you follow
- **Manage** — List the channels linked to your number with roles and subscriber counts

### How it works

1. Run WAHA on a VPS, bound to the local interface (`docker run -p 127.0.0.1:3000:3000 -e WAHA_API_KEY=secret devlikeapro/waha`), and expose it over HTTPS with a reverse proxy (Caddy, Nginx or Traefik) on a domain you control

2. Open WAHA's dashboard, start a session (pick the NOWEB engine to create channels) and scan the QR with your phone (WhatsApp → Linked devices)
3. Subscribe to this server and set your WAHA URL + optional API key
4. Ask your agent to post — e.g. "publish today's release notes to our announcement channel"

### Notes

- WAHA is free and open source.
- WAHA emulates WhatsApp Web: automating a channel through it is outside WhatsApp's official API. Use it on your own account and accept the (small, session-based) risk of restrictions.
- You must be OWNER or ADMIN of a channel to post — subscribers are read-only.

### Who is this for?

- **Creators & community managers** — automate announcements, digests and scheduled newsletters
- **Marketers** — monitor competitor channels and reaction analytics programmatically
- **Developers** — wire WhatsApp broadcasting into agents, cron jobs and publishing pipelines


## Available Tools (8)
- **get_channel_preview**: Pass the invite code from a whatsapp.com/channel/<CODE> link or the @newsletter id. Only the preview window is visible; use get_channel_messages for full history of channels you follow.

Preview the latest posts of any public channel without subscribing to it
- **list_channels**: Use it first to find the @newsletter channel id needed for posting; filter with role=OWNER or role=ADMIN — subscribers cannot post.

List WhatsApp Channels linked to the logged-in number (owned, administered or subscribed)
- **get_channel_messages**: Page back in history with before_timestamp set to the oldest timestamp of the previous page; page forward with after_timestamp set to the newest one seen. The channel must be one your number follows — otherwise use get_channel_preview.

Read posts from a channel you are subscribed to, newest first
- **get_channel**: Accepts either a full channel id ("120363...@newsletter") or the invite code — the last path segment of a https://whatsapp.com/channel/<CODE> link. Use it to check subscriber reach before or after posting.

Get one channel profile by newsletter id or invite code, including subscriber count
- **post_channel_media**: file_url must be publicly downloadable — WAHA downloads it server-side before posting. For image/video the optional caption appears under the media; voice posts ignore captions. Requires role OWNER or ADMIN; channel_id ends with "@newsletter".

Publish an image, video or voice post to a WhatsApp Channel from a public file URL
- **post_channel_text**: Requires your role OWNER or ADMIN on the channel — subscribers cannot post. channel_id must end with "@newsletter" (get it from list_channels). Supports normal WhatsApp text formatting; emoji included as-is.

Publish a text post to a WhatsApp Channel you own or administer
- **search_channels**: Paginate with start_cursor using the endCursor from the previous response (recommended limit 50). Useful to monitor competitors or find a channel before subscribing.

Discover public WhatsApp Channels by keyword (like the in-app explore search)
- **create_channel**: The WAHA session must use the NOWEB, WPP or GOWS engine — the default WEBJS engine cannot create channels (posting to an existing channel still works on WEBJS). Keep the name short and unique. Optionally attach a profile picture from any public image URL.

Create a new WhatsApp Channel owned by the logged-in number




## ❓ FAQ

**Q: What is WAHA and why do I need it?**
WAHA is the WhatsApp API server this connector talks to — a free open-source app you run in Docker on your own infrastructure. It keeps your WhatsApp session under your control: no third party ever sees your messages or credentials.

**Q: What do I need to set up before first post?**
Run WAHA on a VPS bound to 127.0.0.1:3000 (docker run -p 127.0.0.1:3000:3000 -e WAHA_API_KEY=secret devlikeapro/waha) and expose it over HTTPS via a reverse proxy (Caddy/Nginx/Traefik) on your own domain. Open WAHA's dashboard at that HTTPS URL, start a session, scan the QR code with the phone that owns your channel, then set WAHA_BASE_URL (https://...) and WAHA_API_KEY in this server's credentials.

**Q: Why do my posts fail with a permissions error?**
Only owners and admins can publish to a channel — subscribers cannot. Run list_channels to check your role, and make sure the channel id you pass ends with @newsletter.

**Q: Is my WhatsApp account safe using WAHA?**
WAHA is self-hosted, so your session stays on your own server and never touches a third party. It emulates WhatsApp Web, which is outside WhatsApp's official terms — keep posting volume human-like (a few broadcast posts, not spam) to minimise restriction risk.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/whatsapp-channels](https://vinkius.com/en/ai-agent-connect/whatsapp-channels)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WhatsApp Channels** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `whatsapp-channels` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WhatsApp Channels** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "whatsapp-channels": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
