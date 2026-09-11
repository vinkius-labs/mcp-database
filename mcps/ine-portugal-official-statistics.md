# INE Portugal Official Statistics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/ine-portugal-official-statistics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Statistics Portugal (INE) official indicator API: CPI, unemployment, population, GDP, wages and hundreds of series broken down by NUTS regions and all 3000+ municipalities — keyless, no registration.

## Description
The **official indicator web service of Statistics Portugal (INE)** — the national statistical authority — as a single MCP server.

### What you can do
- **Latest values** — the most recent figure of any indicator for every territory at once: Portugal (PT), NUTS I/II/III regions and all 3,000+ municipalities
- **Complete series** — full historical time series per indicator and territory (monthly, quarterly or annual)
- **Territory comparisons** — rankings and side-by-side comparisons of municipalities or regions in the latest period
- **Rich metadata** — units, decimal precision, periodicity, period coverage and dimensional breakdowns (PT/EN)
- **Indicator discovery** — find indicator codes through INE datasets on the dados.gov.pt catalog, since INE's own portal has no code-search API

### What lives here
CPI and inflation, unemployment and labour market, population and demographics, GDP and regional accounts, wages and earnings, housing prices, tourism, agriculture, health personnel and much more — the official numbers used by the Portuguese government, ECB and Eurostat.

### Who is this for?
Economists, analysts, journalists, urban planners, researchers, real-estate and market analysts, and AI agents that need the authoritative Portuguese statistic — not a third-party estimate.


## Available Tools (6)
- **compare_territories**: Great for rankings: "municipalities with highest population density", "NUTS III with lowest purchasing power". geocod examples: PT=Portugal, 1106=Lisboa municipality, 1116=Porto, 1=Continente.

Compare an INE indicator across multiple territories in the latest period (rankings)
- **get_indicator_latest**: Ideal for "what is the current CPI/unemployment/population" questions. Payload stays small even for 300+ territories.

Get the LATEST value of an INE indicator for every territory (lightweight)
- **get_indicator_metadata**: g. 0014855): name (PT/EN), unit of measure, decimal precision, periodicity, first/last period, last update and dimensional breakdown (territory hierarchy, other dimensions). Find codes via search_indicator_codes.

Get full metadata of an INE statistical indicator (unit, periodicity, dimensions, period range)
- **get_indicator_trend**: geocod PT = Portugal total; municipality/NUTS codes appear in get_indicator_latest. Only the requested territory is returned. Note: for VERY large indicators (e.g. full CPI family) the historical payload can be slow (30s+) — prefer get_indicator_latest there.

Get an INE indicator's historical series for ONE territory (chronological trend)
- **search_indicator_codes**: gov.pt datasets and extracts indicator codes from INE dataset slugs (format: "...-0014855"). Returns varcd + dataset title + slug. This is the reliable discovery path — INE's portal has no code-search API. Try terms like "indice de precos no consumidor" (IPC), "taxa de desemprego", "populacao residente".

Discover INE indicator codes: search dados.gov.pt for INE datasets whose slug ends in the 7-digit varcd
- **get_indicator_full_series**: Use only when trend/latest/compare are not enough. Data lives in Pref (and Dados for latest-period calls), grouped by period with every territory.

Get the COMPLETE historical series of an INE indicator (all territories, all periods) — large payload


## 💬 Prompt Examples

Here are some examples of how you can interact with the **INE Portugal Official Statistics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which municipality has the most pharmacists per 1000 inhabitants? (INE indicator 0014855)"

**🤖 AI Agent:**
> 📊 **Pharmacists per 1000 inhabitants — latest year (INE 0014855)**

National average (PT): 1.51

Top municipalities:
1. Lisboa — 4.9
2. Coimbra — 3.8
3. Braga — 2.6

Clear university-city pattern. Want the bottom of the ranking or the trend since 2010?

---

**👤 You:**
> "Show me the population trend of the municipality of Porto since 2010"

**🤖 AI Agent:**
> 📈 **Porto municipality (geocod 1116) — population trend**

2010: 237,559 → 2015: 230,111 → 2020: 231,962 → 2023: 231,506

After two decades of decline, Porto stabilised in the 2020s — tourism-driven immigration and student retention offset suburban flight. I can compare with Lisboa (1106) or pull the regional NUTS III series.

---

**👤 You:**
> "Find the INE indicator code for inflation and give me the latest CPI value"

**🤖 AI Agent:**
> 🔎 **Discovery + latest value**

Searched dados.gov.pt for INE datasets about inflation → found indicator **0007113** (Consumer Price Index, monthly).

Latest reading (PT, last published month): annual variation 2.4%, with food and housing as main contributors. Want the 12-month series or a sub-index breakdown?


## ❓ FAQ

**Q: Do I need an API key or registration?**
No. INE's indicator web service is public — every tool works without authentication. (Note: INE also documents a richer API that does require registration; this MCP uses the keyless indicator service.)

**Q: How do I find the 7-digit indicator code?**
Use search_indicator_codes — it queries dados.gov.pt for INE datasets and extracts the varcd embedded in their resource URLs. You can also browse the INE website's bddExplorer and pick the code from the URL.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/ine-portugal-official-statistics](https://vinkius.com/en/ai-agent-connect/ine-portugal-official-statistics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **INE Portugal Official Statistics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ine-portugal-official-statistics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **INE Portugal Official Statistics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ine-portugal-official-statistics": {
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
