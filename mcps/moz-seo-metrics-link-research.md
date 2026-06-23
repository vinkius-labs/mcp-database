# Moz (SEO Metrics & Link Research) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moz-seo-metrics-link-research)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Manage SEO metrics via Moz — audit Domain Authority (DA), analyze backlinks, and track site rankings.

## Description
Connect your **Moz API** account to any AI agent and take full control of your search engine optimization, link research, and competitive intelligence through natural conversation.

### What you can do

- **Authority Orchestration** — Retrieve precise Domain Authority (DA) and Page Authority (PA) scores for any URL or root domain to understand ranking potential directly from your agent
- **Backlink Audit** — List incoming and outgoing links for specific domains, extracting source URLs, anchor texts, and equity boundaries to identify high-value linking opportunities
- **Competitive Intelligence** — Compare multiple target domains simultaneously to retrieve side-by-side metrics including spam scores and literal link counts securely
- **Anchor Text Analysis** — Extract the literal distribution of anchor text across your backlink profile to understand semantic density and keyword relevance natively
- **Top Pages Discovery** — Query the most internally and externally linked pages within a domain, sorted by Page Authority, to identify high-equity content assets
- **Global Web Rankings** — Access globally tracked lists of top root domains and pages based on Moz's massive link index to benchmark against industry leaders
- **Usage Monitoring** — Track your API row consumption and remaining quotas in real-time to manage your research budget and avoid automated service halts

### How it works

1. Subscribe to this server
2. Enter your Moz API V3 Token
3. Start optimizing your search presence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SEO Specialists** — analyze domain authority and audit link equity through natural conversation without manual keyword research tools
- **Digital Marketers** — track backlink profiles and monitor competitive site metrics directly from your workspace
- **Content Strategists** — identify top-performing pages and analyze anchor text distributions efficiently to guide content production


## Available Tools (10)
- **get_url_metrics**: 0 metrics defining explicitly domain rankings and literal link equity boundaries.

Get Moz API V3 Domain Authority (DA) Page Authority (PA) spam scoring and mapped exact link counts
- **get_incoming_links**: Get explicit incoming backlinks hitting a specific domain mapping Moz API link index
- **get_outgoing_links**: Get explicit outgoing external links originating from a target mapping outbound anchor texts
- **get_top_links**: Get explicitly top-ranked backlinks mapped directly onto a domain sorted primarily by Domain Authority
- **get_anchor_text**: Analyze literal anchor text distribution matching backlinks that point to an explicit domain
- **get_linking_domains**: Get summarized root linking domains hitting specific bounds
- **get_top_pages**: Query top-performing literal pages existing inside an explicit domain sorted by highest internal linking/PA
- **global_top_pages**: Extract static global Top Pages across entire web indexed by Moz metric systems
- **global_top_domains**: Extract static global Top root Domains evaluating worldwide highest DA metrics
- **get_usage**: Check running quota tracking for current Moz API rows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moz (SEO Metrics & Link Research)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get Moz metrics for 'moz.com' and 'ahrefs.com'"

**🤖 AI Agent:**
> Retrieving metrics… For 'moz.com', the DA is 91 and the Spam Score is 1%. For 'ahrefs.com', the DA is 90 with a 2% Spam Score. Both domains show very high authority. Would you like me to compare their top incoming backlinks?

---

**👤 You:**
> "List the top 5 incoming links for 'stripe.com' sorted by authority"

**🤖 AI Agent:**
> Retrieving backlinks… I've identified the top sources: 1) apple.com (PA: 95), 2) nytimes.com (PA: 94), 3) github.com (PA: 92), 4) wired.com (PA: 90), and 5) techcrunch.com. These high-equity links contribute significantly to Stripe's DA. Would you like to see the anchor text for these links?

---

**👤 You:**
> "Show me the anchor text distribution for 'vercel.com'"

**🤖 AI Agent:**
> Analyzing anchor text… For 'vercel.com', the distribution is: 'vercel' (45%), 'next.js' (22%), 'deploy' (12%), 'https://vercel.com' (8%), and 'frontend cloud' (5%). The profile looks very natural with strong brand association. Would you like me to identify which domains use the 'frontend cloud' anchor?


## ❓ FAQ

**Q: What is the difference between DA and PA in Moz?**
Domain Authority (DA) predicts how well a whole website will rank, while Page Authority (PA) predicts the ranking potential of a single page. Your agent can retrieve both metrics using the `get_url_metrics` tool to guide your SEO strategy.

**Q: How do I check the anchor text distribution for my backlinks?**
Use the `get_anchor_text` tool with your target domain. Your agent will retrieve a mapped list of terms and their occurrence counts, helping you identify if your link profile looks natural or over-optimized for specific keywords.

**Q: Can my agent find the best pages on a competitor's site?**
Absolutely. Use the `get_top_pages` tool with the competitor's domain. Your agent will return a list of their highest-authority pages, allowing you to see which content pieces are attracting the most link equity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moz-seo-metrics-link-research](https://vinkius.com/mcp/moz-seo-metrics-link-research)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moz (SEO Metrics & Link Research)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moz-seo-metrics-link-research` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moz (SEO Metrics & Link Research)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moz-seo-metrics-link-research": {
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
