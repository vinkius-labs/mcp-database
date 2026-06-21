# SEO Analyst Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/seo-analyst-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

A startup published 50 blog posts targeting 'high volume keywords.' Six months later: zero organic traffic. Why? Nobody checked indexation — 23 pages had noindex tags from staging. 12 pages cannibalized the same keyword. The site had 89 orphan pages with zero internal links. LCP was 4.8 seconds on mobile. And the 'high volume' keywords had KD 75 against DA 28. This tool forces five SEO axes: technical audit before content, keyword strategy with KD vs DA analysis, content clusters with information gain, backlink profile with competitor gap, and competitive positioning with share of voice.

## Description
## The Problem

1. **Crawl Amnesia** — no technical audit: orphan pages, broken canonicals, CWV failures.
2. **Keyword Vanity** — chasing KD 80 keywords with DA 30. Impossible.
3. **Topical Shallowness** — individual pages, no clusters, no information gain.
4. **Backlink Blindness** — position #1 has 3.8x more referring domains.
5. **Competitive Vacuum** — analyzing in isolation, not against competitors.


## Available Tools (1)
- **validate_seo_analysis**: You must: (1) TECHNICAL — crawl efficiency: indexed pages vs expected, orphan pages, CWV scores per template (not site average), redirect chains (max 1 hop), canonical conflicts, rendering issues (JS-dependent content), (2) KEYWORDS — intent mapping (informational/navigational/commercial/transactional), KD vs DA comparison (only target keywords within 20 DA points of #5 result), SERP feature analysis (featured snippets, PAA, video carousels — can you win them?), cannibalization audit (multiple pages targeting same keyword = signal dilution), (3) CONTENT — pillar-cluster architecture (not orphaned pages), internal linking map (every page reachable within 3 clicks), information gain (what does YOUR content offer that existing SERP results do not?), publishing velocity (consistent cadence, not burst-then-silence), (4) BACKLINKS — referring domain count with DA brackets (DA<10 = junk, DA 10-30 = mid, DA 30+ = quality), anchor text distribution (branded 40-60%, exact match <5%, generic 20-30%), toxic ratio (disavow >5% toxic domains), competitor link gap (how many quality links ahead?), (5) COMPETITIVE — share of voice vs top 5 competitors, SERP overlap %, content velocity comparison (are you publishing faster or slower?), DA gap, realistic win list (keywords where you can realistically reach top 5 within 6 months). If rejected, the analysis has a blind spot — address it before executing strategy.

Structured reflection tool for expert-level SEO analysis — forces systematic auditing across 5 axes that cover the full SEO diagnostic spectrum. Based on Ahrefs/SEMrush audit methodologies, Google Search Console data patterns, and enterprise SEO frameworks for sites with 10K+ pages. Catches Crawl Amnesia (no technical audit of crawl efficiency — Google Search Console shows 85,000 pages indexed. The site has 12,000 actual content pages. 73,000 phantom pages: faceted navigation (/products?color=red&size=M&sort=price — 4 colors × 5 sizes × 3 sorts = 60 combinations per product × 500 products = 30,000 faceted URLs), paginated archives (/blog/page/2 through /blog/page/847), parameter variations (?utm_source=... ?ref=... ?sessionid=...). Google spends 85% of its crawl budget on junk pages. The 12,000 real pages are crawled every 45 days instead of every 3 days. Fix: robots.txt disallow faceted URLs, canonical to non-parameterized versions, noindex on paginated archives beyond page 5, parameter handling in Search Console. Result: crawl budget reclaimed → important pages crawled 15x more frequently), Keyword Vanity (targeting impossible keywords — Site DA: 22. Target keyword: "project management software" — KD 78. Top 5 results: Asana (DA 92), Monday.com (DA 89), Trello (DA 91), Jira (DA 93), ClickUp (DA 84). Probability of ranking in top 10 with DA 22: approximately 0%. Time invested: 6 months of content creation targeting this keyword. Result: page 7. Alternative: "project management for construction teams" — KD 18, 2,400 searches/month. Top 5: DA 35-55 sites. Rankable within 3 months. Revenue potential: 2,400 × 3.2% CTR × 4.5% conversion × $49/mo = $170/month from ONE keyword. Rule: only target keywords where YOUR DA is within 20 points of the #5 result. DA 22 → target KD < 35. Win 50 long-tail keywords before chasing head terms), Topical Shallowness (individual pages without pillar-cluster architecture — The site has 40 blog posts about "project management" — but no structure. 40 orphaned pages competing with each other for the same keyword cluster. Google cannot determine which page is the authority — so it ranks NONE of them. This is keyword cannibalization: 5 pages target "agile project management" — each splits signals (backlinks, clicks, time-on-page) across 5 URLs instead of concentrating on 1. Fix: pillar page "/project-management/agile" (3,000 words, comprehensive). Cluster pages: "/project-management/agile/daily-standup", "/...agile/sprint-planning", etc. Internal linking: every cluster page links to pillar, pillar links to all clusters. Result: Google sees topical authority → ranks the pillar for head term, clusters for long-tail), Backlink Blindness (ignoring link profile quality and competitor gap — Site has 1,200 referring domains. "Great link profile!" Analysis: 800 are directory listings (DA < 10, no traffic). 200 are forum signatures and blog comments (nofollow, zero value). 150 are foreign-language spam sites (toxic — Google penalty risk). 50 are legitimate editorial links (DA 30+, relevant, dofollow). Effective link profile: 50 quality referring domains, not 1,200. Competitor: 3,200 referring domains — 400 are DA 40+ editorial links. Link gap: competitor has 8x more quality links. Priority: disavow 150 toxic domains (penalty prevention), then build 20 editorial links/quarter through original research, data studies, and expert commentary), and Competitive Vacuum (analyzing SEO in isolation, without competitive context — "Our organic traffic grew 15% this quarter!" Competitor A grew 42%. Competitor B grew 28%. The market grew 35%. You grew 15% in a market growing 35% — you LOST market share. Share of Voice: you rank for 340 keywords in top 10. Competitor A: 1,200 keywords. Competitor B: 890 keywords. SERP overlap: you compete with Competitor A on 180 keywords — they outrank you on 165 of them. Without competitive context: "15% growth" feels like success. With competitive context: you are falling behind at an accelerating rate. Action: identify the 50 keywords where competitor ranks #4-#10 but you are #11-#20 — these are winnable with content updates and 5-10 quality backlinks each). Call once per SEO strategy, site audit, or competitive analysis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SEO Analyst Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "The site is accessible and loads fine. We target high volume keywords. We write blog posts about trending topics. Content is king. Our SEO is fine."

**🤖 AI Agent:**
> CRAWL_AMNESIA — Five failures: no indexed pages count, no CWV scores, vanity keywords without KD analysis, individual posts not clusters, 'content is king' ignoring backlinks, no competitive analysis.

---

**👤 You:**
> "Technical: 1,847 indexed (expected 2,100), 89 orphan, LCP 2.1s, INP 145ms, CLS 0.08. Keywords: 'PM tool' KD 72 (HARD vs DA 45), 'PM small teams' KD 38 (WIN). Content: pillar 3,200 words + 12 clusters, bidirectional links, info gain: AI PM section missing from SERP. Backlinks: 342 RD (147 DA>30), anchors safe, toxic 4.2%, gap 89 domains. Competitive: SOV 12.4% vs A 31%, velocity 12/mo vs A 24/mo, DA gap 23, 14 realistic wins identified."

**🤖 AI Agent:**
> SEO_ANALYSIS_PROVEN — All five axes validated at expert level.

---

**👤 You:**
> "Technical: indexed 1,847, CWV passing. Keywords: 'project management' vol 14,800 KD 72, 'best PM tool' vol 8,200 KD 68. Content: 8 blog posts, no clusters. Backlinks: 'we do not do link building, content attracts links.' Competitive: 'our content is good.'"

**🤖 AI Agent:**
> KEYWORD_VANITY — Technical passes. Keywords FAIL: KD 72 and 68 vs DA 45 = both impossible. Target KD ≤ 55. Content needs clusters. 'Content attracts links' is a myth — position #1 has 3.8x more RDs.


## ❓ FAQ

**Q: Why technical audit before content?**
Content on a broken technical foundation gets zero traffic. If pages have noindex, broken canonicals, or 4s+ LCP, Google will not rank them regardless of quality. Fix crawlability, indexation, and CWV first.

**Q: What is KD vs DA analysis?**
Keyword Difficulty (KD) measures how hard to rank. Domain Authority (DA) measures your site strength. Target KD ≤ DA + 10 for realistic wins. KD 75 with DA 30 = impossible. KD 35 with DA 30 = winnable.

**Q: Why do 90% of pages get zero traffic?**
Ahrefs study: 90.63% of pages get zero Google traffic. Causes: targeting impossible keywords, no backlinks, thin content without topical authority, technical issues preventing indexation, no internal linking. The fix: technical audit + realistic keyword targeting + content clusters + link building.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/seo-analyst-prover](https://vinkius.com/mcp/seo-analyst-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SEO Analyst Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `seo-analyst-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SEO Analyst Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "seo-analyst-prover": {
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
