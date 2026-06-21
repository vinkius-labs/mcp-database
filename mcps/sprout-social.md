# Sprout Social MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sprout-social)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Empower your AI with a full social media command center. Draft posts, track global analytics, and master listening topics natively across all brands.

## Description
Bring your **Sprout Social** enterprise command center directly into your artificial intelligence workflow. Stop shifting between code windows and social calendars. With this Vinkius MCP integration, your AI assistant inherits full programmatic capability over your corporate brand identity. From fetching granular interaction analytics or orchestrating new scheduled announcements via a simple markdown prompt, you obtain complete control over global social operations right inside your coding editor environment.

### What you can do

- **Campaign Publishing** — Tell the AI to `create_social_post` across multiple platforms simultaneously, drafting or even queuing content directly by running `list_scheduled_posts`
- **Analytics Tapping** — Command an automatic aggregation of your weekly performance invoking `get_profile_metrics` or isolate specific campaign successes relying on `get_tag_performance`
- **Brand Listening** — Exploit the `get_listening_analytics` action to digest what the global internet is saying about your brand by checking configurations under `list_listening_topics`
- **Profile Auditing** — Keep your brand architecture organized mapping your active nodes through `list_profiles` and verifying structure using `list_profile_groups`

### How it works

1. Subscribe to this AI integration server natively
2. Authorize via your Sprout Social token and your Customer ID
3. Engage your language model internally telling it to draft, schedule, or gather real-time sentiment analysis over recent posts

### Who is this for?

- **Social Media Managers & Analysts** — command your agent to compile raw markdown comparison charts between Twitter and LinkedIn performance seamlessly
- **Marketing Tech Directors** — use LLMs to evaluate specific social text patterns locally looking for hidden success correlations before launching
- **DevSecOps** — rapidly write scripts triggering custom announcements crossing to official PR domains directly using prompt-level commands


## Available Tools
- **create_social_post**: Provide a JSON array of profile_ids, the post text, and an optional scheduled_at time (ISO 8601).

Create and schedule a new social media post
- **get_listening_analytics**: Provide topic_id, start_date (YYYY-MM-DD), and end_date (YYYY-MM-DD).

Get social listening metrics for a specific topic
- **get_profile_metrics**: Provide profile_id, start_date (YYYY-MM-DD), and end_date (YYYY-MM-DD).

Get Sprout Social profile analytics
- **get_tag_performance**: Get performance reports based on Sprout Social tags
- **list_draft_posts**: List draft posts in Sprout Social
- **list_profile_groups**: List Sprout Social organizational groups
- **list_listening_topics**: List social listening topics
- **list_profiles**: ).

List connected Sprout Social profiles
- **list_published_posts**: List published posts for a social profile
- **list_scheduled_posts**: List scheduled posts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sprout Social** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me the list of profiles attached, I need to know which ones are our global Facebook pages."

**🤖 AI Agent:**
> Gathering connected profile roots using `list_profiles`:

1. 📘 **Facebook Fan Page** - 'Global Vinkius Tech' (ID: 100223)
2. 🐦 **X / Twitter** - '@VinkiusGlobal' (ID: 554302)
3. 📘 **Facebook Fan Page** - 'Support EU' (ID: 100889)

You have two primary Facebook targets linked. Would you like to schedule an announcement across `100223` natively?

---

**👤 You:**
> "Tell me the profile metrics for the first week of September on our X/Twitter account."

**🤖 AI Agent:**
> Fetching analytics from `get_profile_metrics` on ID 554302 targeting [2025-09-01 => 2025-09-07]:

- **Total Engagements**: 4,210 (+12% vs prior week)
- **Net Follower Growth**: 154
- **Total Impressions**: 185K

Your X profile sustained healthy organic virality this period. Should I query the specific tags or listening reports?

---

**👤 You:**
> "Create and schedule a new post for our primary account. Output JSON array structure and tell it: 'Big things coming next Friday!' queued for 2025-10-10 at noon."

**🤖 AI Agent:**
> Assembled payload arrays calling `create_social_post` with parameter `profile_ids: ["100223"]` natively bridging string texts:

**STATUS: QUEUED SUCCESS** ✅
**Timestamp Set**: `2025-10-10T12:00:00Z`
**Content Mapped**: "Big things coming next Friday!"

The post successfully resides securely encapsulated within Sprout Social backend ready to automatically clear pipelines at your allocated interval block. Use `list_scheduled_posts` to re-audit if desired.


## ❓ FAQ

**Q: Can the AI really create and publish a post sequentially?**
Yes. Once you gather valid endpoints using `list_profiles`, you can instruct the AI to construct content. When instructed, the bot calls `create_social_post`, supplying your generated text payload and matching the ID, broadcasting it natively. It can also assign scheduled timestamps for delayed publishing.

**Q: How can I extract sentiment from a listening topic intelligently?**
Use the tool `list_listening_topics` to find the exact ID representing a brand trend. Ask the AI: "Diagnose listening id '123' for the past month". It will automatically run `get_listening_analytics`, interpreting the JSON outputs consisting of sentiment ratios, mention volumes, and mapping the sentiment securely inside your chat.

**Q: Do I need to leave a tab logged into Sprout Social open?**
No, this is completely headless. As long as you provided the `SP_TOKEN` and `SP_CUSTOMER_ID` strings globally to your MCP integration parameters, the AI interacts with REST endpoints securely and natively in the background.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sprout-social](https://vinkius.com/mcp/sprout-social)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sprout Social** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sprout-social` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sprout Social** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sprout-social": {
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
