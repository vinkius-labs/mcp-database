# Reddit Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/reddit-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Tap into Reddit's public communities for real-time marketing intelligence — discover trending topics, monitor niches, and analyze sentiment with a free Reddit app.

## Description
Connect any AI agent to Reddit's live public data and transform community conversations into actionable marketing intelligence — with **zero configuration required**.

### What you can do

- **Subreddit Monitoring** — Fetch hot, new, top, rising, or controversial posts from any public community, sorted by time period
- **Global & Scoped Search** — Search all of Reddit or restrict to a specific subreddit by keyword, sorted by relevance, engagement, or recency
- **Multi-Community Feed** — Aggregate posts from multiple subreddits simultaneously into a single ranked feed for niche dashboards
- **Sentiment Analysis** — Pull top comments from any post to understand authentic community reactions, objections, and opinions
- **Subreddit Discovery** — Find relevant communities by topic with subscriber counts so you can prioritize high-impact targets
- **Flair Filtering** — Retrieve posts by flair category (e.g. 'Case Study', 'Question', 'Resource') to filter by content type
- **Popular Communities** — Discover the most active and popular subreddits on Reddit right now
- **Influencer Lookup** — Retrieve public karma and account age for any Reddit user to evaluate content credibility

### How it works

1. Subscribe to this server
2. No credentials needed — start immediately
3. Ask your AI agent to monitor subreddits, search topics, or analyze posts

### Who is this for?

- **Marketing Teams** — track what your target audience is actually saying about your industry, product category, or competitors
- **Content Strategists** — discover high-engagement topics before they go mainstream by monitoring rising posts
- **Brand Managers** — monitor brand mentions and sentiment across relevant communities in real time
- **Growth Hackers** — identify the subreddits where your ideal customers spend time and what problems they discuss most


## Available Tools
- **get_post_comments**: Invaluable for sentiment analysis, understanding community reactions, identifying objections, and surfacing authentic user opinions about products, brands, or topics. Extract the post ID from the permalink URL (the alphanumeric segment after /comments/).

Get comments from a Reddit post for sentiment and opinion analysis
- **search_subreddits**: Use to identify target communities for marketing analysis — e.g., search "crypto" to find r/cryptocurrency, r/Bitcoin, r/altcoins, etc. Returns subscriber counts so you can prioritize.

Discover relevant subreddits by keyword or topic
- **get_posts_by_flair**: Highly useful for filtering by content category — e.g., in r/marketing get only posts with flair "Case Study", "Question", or "Resource". Flairs are community-defined content categories.

Get top posts filtered by a specific flair tag within a subreddit
- **get_multi_feed**: Ideal for creating niche marketing intelligence dashboards — e.g., monitor all of "marketing + entrepreneur + smallbusiness + growthhacking" at once.

Aggregate posts from multiple subreddits simultaneously into a single feed
- **get_popular_subreddits**: Use to discover high-traffic communities and identify where the largest audiences are active.

Get the most popular subreddits on Reddit right now
- **search_reddit**: Essential for competitive intelligence, brand monitoring, topic discovery, and sentiment analysis. Use sort="relevance" for best match, sort="top" with time="week" for most engaged recent content.

Search Reddit posts across all communities or within a specific subreddit
- **get_subreddit_info**: Use to evaluate community size and relevance before targeting it for marketing analysis.

Get metadata and statistics for a subreddit community
- **get_subreddit_posts**: Use for monitoring community conversations, identifying viral content, and tracking engagement in specific marketing niches. Sort by "top" with time="week" for weekly best performers. Sort by "rising" to catch breakout content early.

Get posts from a subreddit sorted by hot, new, top, rising, or controversial
- **get_user_profile**: Useful for influencer identification and evaluating the credibility of content authors.

Get public profile data for a Reddit user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reddit Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the most engaging posts in r/marketing this week?"

**🤖 AI Agent:**
> I fetched the top 25 posts from r/marketing this week. The most engaging post (score: 1,842) is 'How we grew from 0 to 10k email subscribers in 90 days' with 312 comments and a 97% upvote ratio. The second trending topic is around AI content strategy, with 3 posts in the top 10 discussing its impact on SEO.

---

**👤 You:**
> "Search Reddit for discussions about 'AI writing tools' and tell me what people are saying."

**🤖 AI Agent:**
> I searched Reddit for 'AI writing tools' (past week, sorted by top). Found 25 results across 12 subreddits. The dominant sentiment is mixed: r/marketing users praise tools like Claude for strategy work, while r/copywriting shows resistance, with the top post ('AI is killing authentic brand voice') scoring 934 upvotes. r/entrepreneur is more positive, focusing on productivity gains.

---

**👤 You:**
> "Find me the top subreddits where SaaS founders hang out."

**🤖 AI Agent:**
> I searched for 'SaaS founder' communities. Top results: r/SaaS (187k subscribers, 1.2k active now), r/startups (1.1M subscribers), r/Entrepreneur (3.2M subscribers), r/indiehackers (52k subscribers), and r/microsaas (28k subscribers). I recommend starting with r/SaaS for the most targeted audience and r/indiehackers for bootstrapped founders.


## ❓ FAQ

**Q: Do I need a Reddit account to use this?**
You need a free Reddit app. Go to reddit.com/prefs/apps, click 'create app', select 'script', and copy your Client ID and Client Secret. The whole process takes less than a minute and is completely free.

**Q: Can I monitor multiple subreddits at the same time?**
Yes! Use the `get_multi_feed` tool with a comma-separated list of subreddits (e.g. 'marketing,entrepreneur,smallbusiness'). It aggregates posts from all of them into a single ranked feed.

**Q: How do I find which subreddits are most relevant for my niche?**
Use the `search_subreddits` tool with a keyword describing your niche (e.g. 'SaaS', 'fitness', 'crypto trading'). It returns matching communities sorted by subscriber count so you can prioritize the largest ones.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/reddit-intelligence](https://vinkius.com/mcp/reddit-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reddit Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `reddit-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reddit Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reddit-intelligence": {
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
