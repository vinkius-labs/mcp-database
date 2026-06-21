# Shutterstock MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shutterstock)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Equip your AI agent to radically sift through Shutterstock's immense media vault. Search high-quality images, videos, audio, and audit editorial licenses directly from your prompt.

## Description
Grant your AI agent (like Claude or Cursor) absolute visual acquisition dominance over the Shutterstock global media repository. The Shutterstock MCP equips your LLM to act as a fully autonomous art buyer and licensing auditor.

### What you can do

- **Massive Visual & Editorial Espionage** — Rip through catalogs via `search_images`, `search_videos`, and `search_editorial`.
- **Auditory Infiltration** — Audit and preview track loops using `search_audio` and pull their raw BPM profiles via `get_audio_details`.
- **Vault Cartography** — Interrogate your structural asset lockers applying `list_collections` and `get_license_history`.


## Available Tools
- **get_audio_details**: Get metadata for a specific audio track
- **get_image_details**: Get metadata for a specific image
- **get_license_history**: Retrieve the history of licensed assets
- **get_video_details**: Get metadata for a specific video
- **list_collections**: List your image collections
- **search_editorial**: Search for editorial images
- **search_audio**: Search for music tracks and audio clips
- **search_images**: Returns metadata and preview URLs.

Search for images in the Shutterstock library
- **search_videos**: You can filter by quality, frame rate, and duration.

Search for stock video footage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shutterstock** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for high resolution horizontal images containing a golden retriever playing with a stick."

**🤖 AI Agent:**
> Aggressively deploying `search_images` traversing native matrices with keywords "golden retriever playing stick" explicitly locking aspect mapping parameters targeting structurally `horizontal`. Successfully retrieved 5 premium visual entries—would you like me to deeply extract their watermark-free preview addresses natively?

---

**👤 You:**
> "Look up video ID 12345678 and report back its maximum resolution available."

**🤖 AI Agent:**
> Passively evaluating `get_video_details` directly interrogating ID 12345678 rigorously. Underlying JSON matrix explicitly states Native HD structural acquisition maxing natively at rigidly formatted standard strictly recorded natively at exactly 4K (3840x2160).

---

**👤 You:**
> "Find 5 spooky audio tracks that can loop perfectly by using the search_audio protocol securely."

**🤖 AI Agent:**
> Activating query execution parameters exclusively natively via `search_audio` matching explicitly strings 'spooky' heavily. Filtered definitively filtering explicitly identifying structural loops securely yielding exactly 5 ominous soundscapes seamlessly retrieved fully efficiently. Do you require the absolute strict structural IDs subsequently seamlessly?


## ❓ FAQ

**Q: Can the integration forcefully license or automatically purchase an image?**
No. By structural design, this module is strictly bound as an observational and search lens tailored purely around querying assets violently efficiently. It explicitly omits write protocols preventing your autonomous agent from accidentally sabotaging valid corporate wallets or unintentionally mass-licensing redundant data.

**Q: Can it search for specific internal user collections or boards?**
Yes, utilizing the explicit `list_collections` operational protocol, the token directly verifies and systematically grabs all active native groupings created rigidly beneath the account bounding that token natively.

**Q: Is the Editorial access separated structurally from the standard image search?**
Yes aggressively. Because editorial resources operate identically under completely distinct structural usage and strict rights matrices, we forcibly separate standard asset queries (`search_images`) strictly away from the rigorous editorial boundaries specifically bound uniquely under `search_editorial`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shutterstock](https://vinkius.com/mcp/shutterstock)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shutterstock** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `shutterstock` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shutterstock** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shutterstock": {
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
