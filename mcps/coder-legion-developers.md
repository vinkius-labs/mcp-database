# Coder Legion Developers MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/coder-legion-developers)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Connect AI agents to Coder Legion's public developer directory: browse profiles, search by name, skill, location or experience, and open full developer profiles — no account or key needed.

## Description
Give any AI agent read access to Coder Legion's public developer directory — the roster of the community's engineers, with their headlines, skill tags, locations, experience, community roles and stats. No account, no API key: the directory and profile pages are public.

### What you can do

- **Browse the directory** — `list_developers` walks it in pages of 18 profiles, offset pagination
- **Search the community** — `search_developers` combines name, skill, location and minimum years of experience (filters combine with AND)
- **Open a profile** — `get_developer_profile` fetches one developer's full public profile: roles, headline, location, website, joined date, points/badges/connections/followers/following, skills and about text

### How it works

1. Subscribe to this server
2. Ask your agent to list, search or open Coder Legion developer profiles
3. The server reads the public directory pages and returns structured records with each developer's profile URL

### Who is this for?

- **Recruiters and talent teams** — screen the community by skill, location and experience before reaching out
- **Developers** — find peers, mentors or collaborators for a technology or region
- **Founders and DevRel** — map the talent landscape behind the Coder Legion community


## Available Tools (3)
- **get_developer_profile**: g. "Tom Smith" or "stjepan"). Returns the complete profile: name, verified status, community roles, headline, location, website, joined date, points/badges/connections/followers/following stats, skills and the about text. Use it after list_developers or search_developers to dig into a specific person. If the handle does not match a public profile, the tool says so and points back to the directory tools. No credential is required.

Get the full public profile of one Coder Legion developer by handle
- **list_developers**: Each record includes the developer name, verified status, headline, location, years of experience, skill tags and their profile URL. Use it to survey the directory without a specific criterion. To page through results pass start as a multiple of 18 (0, 18, 36, …) — it is an offset, not a page number. No credential is required: the directory is public. The profile URL returned per record is what get_developer_profile expects when converted to a handle.

Browse the public Coder Legion developer directory, page by page
- **search_developers**: Accepts up to four independent filters that combine with AND: name (partial match), skill (matches skill tags such as "Python" or "Prompt Engineering"), location (e.g. "Remote"), and minimum years of experience (1, 3, 5 or 10). Returns matching records with name, verified status, headline, location, experience, skills and profile URL, plus the start offset used for pagination. If a combination returns nothing, drop the narrowest filter (usually skill or location) and retry. No credential is required.

Find Coder Legion developers by name, skill, location or minimum experience


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coder Legion Developers** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find Coder Legion developers with at least 5 years of experience who list prompt engineering as a skill."

**🤖 AI Agent:**
> I searched the Coder Legion directory for the prompt engineering skill with a 5-year minimum experience. N matches came back; the top few include names, verified badges, locations and their other skills. Each has a profile URL — want me to open the most promising one and summarize their full profile?

---

**👤 You:**
> "Show me the next page of the Coder Legion developer directory."

**🤖 AI Agent:**
> Here are profiles 19–36 of the Coder Legion developer directory (18 per page, offset 18): each with name, verified status, headline, location, experience and skill tags. I can continue paging, apply a filter, or open any of these profiles in full.

---

**👤 You:**
> "Open the Coder Legion profile of the developer the directory listed first for a search of Kubernetes skills, and summarize their stats and about text."

**🤖 AI Agent:**
> I searched the directory for the Kubernetes skill, took the first listed developer, and opened their profile. Summary: verified status, community roles, points and followers, location, join date, website, their headline, the top of their about text, and their full skill list. If you want, I can do the same for the next developers on that list.


## ❓ FAQ

**Q: Do I need an account or API key?**
No. The Coder Legion developer directory and developer profile pages are public, so this connection is keyless — subscribe and use it. The separate Coder Legion connection covers the authenticated API surface (posts, jobs, series, groups, tags), which is where an API key is needed.

**Q: What data does a directory record include?**
Each record has the developer's name, verified badge status, headline, location, years of experience, skill tags and the URL of their public profile. The profile tool adds community roles (with descriptions), website, join date, stats (points, badges, connections, followers, following), the full skill list and the about text.

**Q: How does search work, and what if a search returns nothing?**
Filters combine with AND: name (partial match), a skill tag, a location, and a minimum years of experience (the directory supports 1, 3, 5 or 10). Results are paged by offset in groups of 18. When a combination comes back empty, drop the narrowest filter (usually the skill or the location) and retry — the tool tells the agent exactly that.

**Q: What happens if I pass a handle that does not exist?**
The tool returns a clear "profile not found" error that points back at the directory tools, so the agent recovers by listing or searching first and then opening one of the returned profile URLs. Transient page-load failures surface as a retryable error instead of a crash.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/coder-legion-developers](https://vinkius.com/en/ai-agent-connect/coder-legion-developers)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Coder Legion Developers** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coder-legion-developers` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coder Legion Developers** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coder-legion-developers": {
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
