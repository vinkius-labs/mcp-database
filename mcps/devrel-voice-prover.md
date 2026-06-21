# DevRel Voice Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/devrel-voice-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

AI agents write developer content that sounds like a press release. This tool forces authentic developer-to-developer voice: community-aware context, value over features, actionable code paths, and genuine engagement. No corporate speak, no feature dumps.

## Description
AI agents write developer communications that sound like marketing press releases. They use corporate buzzwords instead of technical language, list features without explaining why developers care, ignore community context, announce without providing actionable paths, and produce generic content that could be from any company.

### The Problem

AI-generated DevRel content fails on five axes:

- **Corporate speak** — "We are excited to announce our innovative, best-in-class solution." Developers tune out immediately. DevRel speaks like a senior engineer explaining to a peer.
- **Feature dumps** — "We added WebSocket support. We added dark mode. We added..." Lists WHAT without explaining WHY. Developers don't care about features — they care about problems solved.
- **Community deafness** — Announces in a vacuum without referencing the GitHub issues, Discord threads, or feedback that drove the change. DevRel responds to community signals, not corporate calendars.
- **No action path** — "Try it out!" is not DevRel. DevRel provides: runnable code example, migration command, docs link, 3-step quickstart, and feedback channel.
- **Template voice** — Generic, interchangeable content. If you replace the brand name with a competitor's and the post still works, it's not authentic DevRel.

### How It Works

5 Decision Pivots validate authentic developer communication:

1. **developerVoice** — Developer-to-developer tone? No "excited to announce", no "innovative", no "best-in-class". Direct, technical, honest.
2. **communityAwareness** — References specific community signals? GitHub issue numbers, Discord threads, feedback votes.
3. **valueArticulated** — Explains WHY developers care? Pain eliminated, workaround removed, workflow changed.
4. **actionablePath** — Runnable code, migration steps, docs link, quickstart, feedback channel.
5. **authenticEngagement** — Personality, vulnerability, specific references, continuity.


## Available Tools
- **validate_devrel_voice**: DevRel is a conversation between an engineer and their peers — not a press release. You must: (1) DEVELOPER VOICE — speak like a senior engineer to a peer. Zero corporate speak: no "excited to announce," no "innovative solution," no "best-in-class," no "leverage," no "synergy," no "empower," no "game-changing," no "seamless experience." Say "We shipped X because you asked" with the issue number, (2) COMMUNITY CONTEXT — reference SPECIFIC community signals: GitHub issues (#number), Discord thread links, feedback board vote counts, conference conversations. "The community wanted this" is NOT context — cite the source, (3) DEVELOPER VALUE — explain WHY developers care, not just WHAT changed. For each feature: what PAIN does it eliminate? What was the WORKAROUND? How does their DAILY workflow change? "We added X" is a feature dump, (4) ACTION PATH — runnable code example (not pseudocode), migration command with output, direct docs link, 3-step quickstart, feedback channel. "Try it out" is not an action path — show the code, (5) AUTHENTIC ENGAGEMENT — personality, vulnerability, specific references, continuity with previous conversations, human details. If you swap the brand name and the post still works, it is template voice. If rejected, your content reads as marketing, not DevRel.

Structured reflection tool for authentic developer relations communication. DevRel is NOT marketing — it is the bridge between product and community. Forces community-grounded context, value articulation (WHY not just WHAT), actionable paths with runnable code, and authentic voice. Catches Corporate Speak ("We are excited to announce our innovative solution" — developers stop reading at "excited to announce." Say "We shipped X because you asked" with a link to the GitHub issue), Feature Dumps ("We added X, Y, Z" without explaining WHY developers care — what pain disappeared? What workaround is eliminated? How does their daily workflow change?), Community Deafness ("The community wanted this" without citing specific signals — which GitHub issues? Which Discord threads? Which feedback votes? No citations = no credibility), Missing Action Path ("Try it out!" is not an action path — show the install command, the import, the minimal working example. Every DevRel piece must answer "What do I DO now?"), and Template Voice (if you swap the brand name and the post still works, it is template voice — no personality, no specific references, no vulnerability, no human details). Call for changelogs, release notes, blog posts, tutorials, migration guides, and announcements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DevRel Voice Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We are thrilled to announce v3.0 of our innovative platform! This game-changing release features a best-in-class API, seamless integrations, and a robust, scalable architecture. Try it today!"

**🤖 AI Agent:**
> Verdict: CORPORATE_SPEAK. Every sentence is a marketing buzzword: 'thrilled', 'innovative', 'game-changing', 'best-in-class', 'seamless', 'robust and scalable'. This reads like a LinkedIn ad, not DevRel. No community context (why v3?), no developer value (what problems solved?), no code (how to migrate?), no feedback channel. Rewrite: 'v3.0 is live. The new API resolves the auth token race condition from issue #189. Migration: `npm install @sdk@3.0.0` — see docs.example.com/v3/mig...

---

**👤 You:**
> "Content: changelog for SDK v2.4. Community: issues #312 and #345 reported auth token expiration wasn't handled gracefully — users got silent 401s with no error message. 23 upvotes on feedback board. Value: SDK now auto-refreshes tokens before expiration and surfaces clear error messages with retry guidance when refresh fails. Before: developers had to build their own token refresh logic and catch opaque 401s. Now: zero-config token lifecycle management. Code: `import { createClien..."

**🤖 AI Agent:**
> Verdict: DEVREL_PROVEN. Developer voice (direct, technical, no buzzwords). Community-aware (issues #312, #345, 23 upvotes). Value articulated (before: manual token refresh + opaque 401s → now: zero-config auto-refresh). Action path (runnable code, opt-in flag, no breaking changes). Authentic (specific issue numbers, before/after comparison, honest about the problem). This is how DevRel communicates. Ship it.

---

**👤 You:**
> "v2.5 release notes. We heard from the community about these needs. Added: GraphQL subscriptions, new rate limiter middleware, database connection pooling, improved error messages, dark mode for dashboard. These features make the platform better. Try them out and let us know what you think!"

**🤖 AI Agent:**
> Verdict: FEATURE_DUMP. Developer voice is acceptable (no buzzwords), community vaguely referenced ('we heard from the community' — but WHICH community signals? No issue numbers, no Discord threads, no feedback votes). Critical failure: pure feature list without WHY. 'Added GraphQL subscriptions' — SO WHAT? Why does a developer care? Was polling killing performance? Was issue #189 about real-time updates? 'Improved error messages' — improved HOW? Before: 'Error 500'. After: 'Postgr...


## ❓ FAQ

**Q: Does this tool write DevRel content?**
No. The agent writes the content. The tool VALIDATES that it communicates like authentic DevRel — developer voice, community awareness, value articulation, actionable paths, and authentic engagement. It catches the five failure modes that make AI-generated developer communications sound like press releases.

**Q: What types of content does it validate?**
Changelogs, release notes, blog posts, tutorials, migration guides, breaking change notices, community updates, retrospectives, roadmap updates, incident postmortems, feature announcements, deprecation notices, getting started guides, and API/SDK updates. Each type has different tone, urgency, and structure requirements that the tool validates.

**Q: Why does the tool reject 'We are excited to announce'?**
Because developers don't care about your excitement — they care about their problems. 'We are excited to announce' is corporate speak that signals 'marketing wrote this.' DevRel says: 'We shipped WebSocket support because issue #247 showed polling was killing your API rate limits. Here's how to migrate in 3 steps.' Direct, technical, problem-focused. That's what builds trust.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/devrel-voice-prover](https://vinkius.com/mcp/devrel-voice-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DevRel Voice Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `devrel-voice-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DevRel Voice Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "devrel-voice-prover": {
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
