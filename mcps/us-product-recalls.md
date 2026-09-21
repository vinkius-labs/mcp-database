# US Product Recalls MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/us-product-recalls)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [shopping](../categories/shopping.md)

Whether the US Consumer Product Safety Commission has recalled a product — check a brand or model against every recall since 1973, and read the full notice.

## Description
Connects an AI agent to the US Consumer Product Safety Commission's recall database — the agency record of every product the commission has pulled from shelves, from 1973 to today.

### What you can do

- **Check a product** — a brand, a model or a barcode, matched across product names, recall titles, companies and UPCs, so "Char-Broil", "Bistro Pro" and the same grill's number all reach the same notices
- **Read one recall** — the products with unit counts, every hazard named, whether injuries were reported and the summary of them, the remedy in the agency's words, who made and imported it, where it sold and for how much
- **See what's new** — every recall published inside a window of days, newest first
- **Browse by hazard** — what has been recalled for choking, fire, lead or a tip-over risk, optionally from one company or with injuries reported
- **Read a period** — how many recalls, which remedies dominate, which companies recur, without listing the notices

### Why it matters

The agency's search interface has traps that this server accounts for. Three documented filters — hazard, UPC and country — return zero for every value, including values present verbatim in the data, so a naive client concludes nothing was ever recalled for choking. A fourth set of parameters is silently ignored and returns the entire ten-thousand-record corpus as if it matched. Neither produces an error; both produce a plausible-looking wrong answer.

Here the broken filters are never sent: hazards and UPCs are matched against the record's own text locally, and a query the agency ignored is refused rather than answered. Beyond filtering, the record is free text where a human would expect a number — the unit count reads "About 10,605 (In addition, 342 were sold in Canada)" — and a recall that reports no injuries phrases it eight different ways, which this server reads as no injuries rather than as an injury report.


## Available Tools (5)
- **check_product**: Give a product name, a brand, a model or a recall number — anything from two characters up. The term is matched across product names, recall titles and descriptions, the companies involved and the UPC list, so "Char-Broil", "Bistro Pro" and a barcode all reach the same notices. Each match reports the recall number and date, what was recalled, roughly how many units, whether injuries were reported, and what the agency told buyers to do. The database covers recalls the CPSC published from 1973 to today, and only recalls — an absence means the agency has not recalled anything under that term, not that the product is safe: a product under investigation, or recalled by another agency such as the FDA or NHTSA, will not appear here. Results are paginated with offset and amount.

Whether the US Consumer Product Safety Commission has recalled a product — the safety check before you buy, keep or gift something
- **recent_recalls**: Give days for a rolling window ending today, or an explicit date_start and date_end in YYYY-MM-DD form for a specific period; both bounds are inclusive. The default window is 30 days, which is roughly the agency's cadence. Each row is the short form — number, date, products, unit count, whether injuries were reported and the remedy — and get_recall carries the full notice. Results are paginated with offset and amount.

The recalls the CPSC has published inside a window of days — what was pulled from shelves recently, newest first
- **search_recalls**: Company, product and remedy are substring matches pushed to the agency's own search; hazard is matched against the words of the hazard description locally, because the agency's hazard filter does not work, so "fire" finds "fire hazard" and "catch fire" but nothing that only implies heat. injuries_reported true keeps recalls where injuries were actually reported and false keeps those where the agency wrote "none reported" — the agency phrases a no-injury recall eight different ways and this accounts for all of them. Give a date range in YYYY-MM-DD to bound the query; an unbounded search across fifty years is slow and mostly noise. Results are paginated with offset and amount.

The CPSC recall database filtered by hazard, company, product, remedy, date and whether injuries were reported
- **summarize_recalls**: Give days for a rolling window or an explicit date_start and date_end in YYYY-MM-DD form. The response counts recalls by month, by remedy offered, and by company, and reports how many had injuries reported and roughly how many units were affected. Unit totals are the agency's own "about N" figures added together, so they are an approximation of the announced count, not an audited number; a company appearing several times had several distinct recalls.

The shape of a recall period without the list — how many, which hazards and remedies dominate, and which companies recur
- **get_recall**: The number is four to six digits, sometimes with one trailing letter, and appears on the agency's notice and in its web address. The response carries the products with their unit counts, every hazard the agency named, whether injuries were reported and the summary of them, the remedy in the agency's words and the options it offered, who made and imported it, where it was sold and for how much, and the consumer contact line. A number that matches nothing reports that plainly rather than guessing.

Everything the CPSC published about one recall — the products, the hazard, the injuries, the remedy and who to contact, by recall number


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Product Recalls** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I'm about to buy a used Char-Broil Bistro Pro electric grill from a neighbour. Has it ever been recalled?"

**🤖 AI Agent:**
> Let me check the product against the recall database — the name is matched across product names, titles, brands and UPCs, so the model name or the brand alone is enough. If there's a recall I'll give you the number, the date, what the hazard is and what the agency told owners to do.

---

**👤 You:**
> "My sister is expecting a baby and I want to gift her a secondhand rocker. How do I make sure it's not one of the ones that were recalled?"

**🤖 AI Agent:**
> Give me the brand and model — or the recall number if the seller has the notice — and I'll check it. If you only have a category, I can search the hazard text for the infant-product terms that matter, like suffocation or fall, and list what was recalled and why.

---

**👤 You:**
> "What did the US recall last month? Just give me an idea of the scale, not every notice."

**🤖 AI Agent:**
> I'll summarise the month rather than list it — the count, how many had injuries reported, roughly how many units were affected, and the split by remedy and by company, which tells you whether it was a few big recalls or many small ones.


## ❓ FAQ

**Q: I searched for a product and got nothing back. Does that mean it's safe?**
It means the commission has not recalled anything under that term, which is a weaker statement. This database holds recalls only, and only those the CPSC issued — products under investigation, products recalled by another agency such as the FDA or NHTSA, and products nobody has reported harm from yet are all absent. Treat an empty answer as "no recall on file" and read the hazard description on the product itself.

**Q: Why does a hazard search match words instead of categories?**
Because the agency's own hazard filter is broken: it returns zero for every value asked of it, including values that appear verbatim in the data, and its hazard-type field is empty on every record. The usable text is the hazard description itself, written in prose, so the search matches your term against those descriptions — "fire" finds "fire hazard" and "catch fire", but a recall that only implies heat will not match. Use several terms if you want to be thorough.

**Q: What counts as a recall with reported injuries?**
A recall whose injury field carries an actual account of harm. Roughly one recall in six phrases a no-injury outcome eight different ways — "None reported", "None reported.", "No incidents or injuries have been reported." and five others — and testing whether the field is simply non-empty counts those as injuries. This server recognises all eight and reports them as no injuries, so filtering to reported injuries keeps only recalls where the agency described harm.

**Q: Why are the unit counts described as approximate?**
Because the agency publishes them as free text, not as a number. A real entry reads "About 10,605 (In addition, 342 were sold in Canada)" and another "About 7,200 (In addition, about 370 were sold in Canada)". The first figure is taken as the headline count and the full phrase is kept beside it, so you see what the agency actually wrote. Adding those first figures across a year gives the order of magnitude, not an audited total.

**Q: Do I need an API key or an account?**
No. The commission publishes this database openly and the server reads it without authentication. There is no key to obtain, no quota to manage and no sign-up step.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/us-product-recalls](https://vinkius.com/en/ai-agent-connect/us-product-recalls)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Product Recalls** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-product-recalls` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Product Recalls** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-product-recalls": {
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
