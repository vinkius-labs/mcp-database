# NASA Mars — Rover Photos from the Red Planet MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nasa-mars-rover-photos-from-the-red-planet)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Browse 800,000+ photos taken on the surface of Mars by NASA rovers Curiosity, Opportunity, and Spirit — filter by sol, Earth date, or camera. Access mission manifests and the latest images beamed directly from the Martian surface.

## Description
Direct access to 800,000+ photos from the Martian surface.

### Rovers
- **Curiosity** (2012-present) — Still active! 7 cameras
- **Opportunity** (2004-2018) — 15 years, 45 km traveled
- **Spirit** (2004-2010) — Twin of Opportunity

### Cameras
FHAZ (front), RHAZ (rear), NAVCAM (navigation), MAST/PANCAM (panoramic), CHEMCAM, MAHLI (hand lens), MARDI (descent)


## Available Tools (4)
- **get_mars_photos**: Filter by camera: FHAZ (front hazard), RHAZ (rear hazard), MAST (mast), CHEMCAM, MAHLI, MARDI, NAVCAM. Curiosity has 800K+ photos.

Get Mars rover photos by sol number and camera
- **get_mars_photos_by_date**: Easier than using sol numbers. Works with all three rovers.

Get Mars rover photos by Earth date
- **get_mars_manifest**: Essential for understanding what data is available.

Get the mission manifest for a Mars rover
- **get_mars_latest**: Curiosity is still active and sending new photos. Opportunity and Spirit missions have ended but their full archives are available.

Get the most recent photos from a Mars rover


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NASA Mars — Rover Photos from the Red Planet** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the latest photos from Curiosity on Mars"

**🤖 AI Agent:**
> 🔴 **Curiosity — Latest Photos**

Sol 4150 | Earth Date: 2026-04-02
📸 12 new images from 3 cameras

1. NAVCAM — Panoramic view of Mt. Sharp
2. MAST — Rock formation detail
3. CHEMCAM — Laser target analysis

Curiosity has taken 850,000+ photos since landing Aug 6, 2012.

---

**👤 You:**
> "Find panoramic photos taken by Opportunity in 2010."

**🤖 AI Agent:**
> I found several panoramic shots taken by Opportunity's PANCAM in 2010. Notably, on Sol 2450 (Dec 2010), the rover captured a stunning 360-degree view of the Santa Maria crater.

---

**👤 You:**
> "How many photos did Spirit send back before its mission ended?"

**🤖 AI Agent:**
> The Spirit rover sent back a total of 124,838 photos from the Martian surface before communication was lost on Sol 2210 (March 22, 2010).


## ❓ FAQ

**Q: Is Curiosity still active on Mars?**
Yes! Curiosity has been active since August 6, 2012 and continues to send new photos and science data. Opportunity operated for 15 years (2004-2018), Spirit for 6 years (2004-2010).

**Q: Can I search photos by Earth date instead of Martian sol?**
Yes, the server supports querying by both Earth date (e.g., '2023-11-20') and Martian Sol (the number of Martian days since the rover landed) for flexibility.

**Q: Which cameras are available on the rovers?**
Available cameras include FHAZ (Front Hazard), RHAZ (Rear Hazard), NAVCAM (Navigation), MAST (Mast Camera), CHEMCAM (Chemistry and Camera), and MAHLI (Mars Hand Lens Imager).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nasa-mars-rover-photos-from-the-red-planet](https://vinkius.com/mcp/nasa-mars-rover-photos-from-the-red-planet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NASA Mars — Rover Photos from the Red Planet** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nasa-mars-rover-photos-from-the-red-planet` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NASA Mars — Rover Photos from the Red Planet** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nasa-mars-rover-photos-from-the-red-planet": {
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
