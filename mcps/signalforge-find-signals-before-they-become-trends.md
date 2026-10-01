# SignalForge — Find signals before they become trends MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/signalforge-find-signals-before-they-become-trends)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [research](../categories/research.md)

Keyless research intelligence: forge early signals from OpenAlex, Crossref, OpenAIRE, Europe PMC, arXiv, CORDIS and an experimental USPTO patent leg — publications, preprints, EU projects, funding, and a best-effort patent layer.

## Description
SignalForge is not a research connector. It forges signals: one call fuses seven public, keyless sources into a single radar view of where a field is moving — before it becomes a trend.

### What you can do
- **signal_scan** — the forge: OpenAlex works and patents, Crossref with funding metadata, arXiv preprints, Europe PMC (biomedical + preprints), OpenAIRE EU projects and an experimental USPTO leg, each contained so one failure never fails the scan
- **openalex_trend** — per-year publication momentum rendered as ASCII bars with the growth percentage; the core early-signal tool
- **openalex_search** / **openalex_topics** — corpus size, citations, topic clusters to monitor
- **crossref_search** — publications filtered by funder DOI: who is investing in a field
- **openaire_search** — EU-funded projects (CORDIS/EC aggregated) and their publications, with green/open-access flags
- **europepmc_search** — biomedical papers and preprints (source PPR), the fastest layer for clinical research
- **arxiv_emerging** — newest submissions, days old, with abstract and PDF
- **cordis_project** — a full EU project fact sheet: programme, grant ID, EU contribution, coordinator, objective
- **patent_signals** — filing activity (best-effort: OpenAlex patent index is currently empty + experimental USPTO leg), the commercial-intent layer ahead of products

### Who is this for
Researchers tracking a field, investors spotting technology inflection, R&D teams deciding where to allocate effort next quarter. No API key anywhere — every source is public.


## Available Tools (10)
- **openalex_topics**: OpenAlex topic and concept clusters matching a keyword, each with its own corpus size and citation count — the discrete "channels" to monitor in a field
- **cordis_project**: g. https://cordis.europa.eu/project/id/101055743). CORDIS's search backend is not anonymously reachable, so keyword discovery of projects flows through openaire_search (resource='projects'); use this tool to open one specific project.

European Union innovation project fact sheet from the server-rendered CORDIS public page: programme, funder, grant agreement ID, EU contribution, coordinator, dates, objective and the CORDIS DOI
- **crossref_search**: g. "10.13039/501100004552" for a national agency) to list what they fund; without it, query.bibliographic free-text search applies. Use it to answer "who is investing here?"

Crossref publication metadata keyless: DOI, authors, journal, type and — the differentiator — funding metadata (funder names), so you can see which funders are backing a field
- **europepmc_search**: sort='citations' ranks by impact instead of recency.

Europe PMC biomedical search keyless: journal articles and preprints (source PPR, filter PUB_TYPE:Preprint), with DOI, PMID, journal and abstract snippets. Biomedical fields are where Europe PMC adds preprint volume OpenAlex does not carry
- **openaire_search**: Keywords are ANDed across words by OpenAIRE — keep them short.

OpenAIRE EU research intelligence keyless: publications (with green/open-access flags, subjects, abstracts) and EU-funded projects (CORDIS/EC aggregated) with code, funder provider, dates and summary
- **openalex_search**: sort=date surfaces the freshest works (emerging signals); sort=citations surfaces what already moved the field.

Search 250M+ OpenAlex scholarly works keyless: title, authors, institution, abstract and citations, sorted by citations (default) or by date. Returns total corpus size — the cheapest "is this a hot field" number
- **openalex_trend**: A field with a small absolute count but steep recent growth is exactly the early signal to flag. Counts are title+abstract matches, not exact topic labels.

Momentum signal: per-year OpenAlex publication counts for a keyword, rendered as ASCII bars, plus the growth percentage across the window. The core "find signals before they become trends" tool
- **patent_signals**: This layer is best-effort: the USPTO leg is experimental (keyless access ends 2026-11-07, backend is WAF-restricted, may report unavailable) and the OpenAlex public type:patent index is currently empty — expect 0 OpenAlex patents until a keyless patent source is added.

Patent signals, best-effort and keyless: OpenAlex type:patent matches (its public index is currently empty, so expect 0) plus an EXPERIMENTAL USPTO Patent Public Search leg that degrades gracefully — keyless access ends 2026-11-07. Patent filing activity is the commercial-intent layer ahead of products
- **signal_scan**: Returns per-source status (ok / degraded / unavailable) plus top signals per source. For per-year publication momentum use openalex_trend; for a deep dive into one source use its dedicated tool. The USPTO leg is experimental and may report unavailable — OpenAlex (patents) already covers patent signals.

Forge a research signal scan across seven public, keyless sources at once: OpenAlex publications and patents, Crossref (with funding metadata), arXiv preprints, Europe PMC (biomedical), OpenAIRE EU projects, and an experimental USPTO patent leg. Each source is contained: one failing source degrades its own leg, never the scan
- **arxiv_emerging**: Pair with openalex_trend to confirm the momentum the fresh papers ride on.

arXiv emerging-research radar keyless: newest submissions matching a term (default) or most relevant ones, with abstract, categories, authors and PDF link. This is the freshest layer — days, not months, old


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SignalForge — Find signals before they become trends** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Any early signals in solid-state batteries?"

**🤖 AI Agent:**
> signal_scan forges the full radar: freshest OpenAlex works, patent filing activity (best-effort leg), latest arXiv preprints, biomedical cross-overs in Europe PMC, EU projects funding the space and Crossref funders — each source marked ok/degraded/unavailable so you know how much to trust it.

---

**👤 You:**
> "Which fields are accelerating right now in AI safety?"

**🤖 AI Agent:**
> Run openalex_trend on 2–3 candidate topics (e.g. 'interpretability', 'mechanistic alignment', 'evaluation of large models'); the per-year bars and the growth percentage rank momentum, and openalex_topics breaks the winners into monitorable sub-topics.

---

**👤 You:**
> "Who in the EU is funded to work on green hydrogen?"

**🤖 AI Agent:**
> openaire_search with resource='projects' and term 'green hydrogen' lists the EU-funded projects (codes, funders, dates, summaries). Open one with cordis_project for the full fact sheet: EU contribution, coordinator, participant count and objective.


## ❓ FAQ

**Q: Do I need an API key?**
No. OpenAlex, Crossref, OpenAIRE, Europe PMC, arXiv and the CORDIS public pages are all keyless. The USPTO Patent Public Search leg is experimental and keyless only until 2026-11-07, when USPTO makes an account mandatory — that leg degrades to a structured unavailable note, and no keyless patent fallback exists today (OpenAlex public type:patent index is empty, probed 2026-09-30), so the patent layer is best-effort.

**Q: What happens when one source is down?**
Every source is an independent leg. signal_scan runs all legs in parallel and contains each failure inside its own leg — the report marks that leg 'unavailable' with the reason and returns the rest. A source under rate limit is marked 'degraded' with a retry hint instead of failing the call.

**Q: Why is The Lens not a source?**
www.thelens.org was observed parked (a GoDaddy for-sale redirect) in September 2026, so the platform was deliberately excluded. The patent layer The Lens offered is not covered by any keyless source today: OpenAlex public type:patent index is empty (0 records, probed 2026-09-30) and the USPTO leg is experimental, keyless only until 2026-11-07.

**Q: How do I see EU-funded projects on a keyword?**
CORDIS's own search backend is not anonymously reachable, so keyword discovery of EU projects flows through OpenAIRE projects (which aggregates CORDIS and EC grants). Pick a project code from openaire_search (resource='projects') and open its full fact sheet with cordis_project.

**Q: Is there rate limiting?**
OpenAlex rate-limits anonymous bursts (429 with retry-after). SignalForge serialises all OpenAlex calls in one process and spaces per-year trend reads, so a scan or trend stays inside the anonymous window; when a limit is hit the leg reports 'degraded' with a retry hint instead of erroring.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/signalforge-find-signals-before-they-become-trends](https://vinkius.com/en/ai-agent-connect/signalforge-find-signals-before-they-become-trends)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SignalForge — Find signals before they become trends** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `signalforge-find-signals-before-they-become-trends` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SignalForge — Find signals before they become trends** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "signalforge-find-signals-before-they-become-trends": {
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
